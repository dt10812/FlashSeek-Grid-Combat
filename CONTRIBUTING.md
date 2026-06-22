# Contributing to FlashSeek: QA & Bug Testing Guide

Thank you for helping test **FlashSeek: Grid Combat**! To maintain a high standard of architectural stability, we use a rigorous, data-driven QA process. 

If you encounter a performance drop, an asset failure, a hardware conflict, or a gameplay exception, please follow this guide to document it and open a **GitHub Issue**.

---

## Pre-Submission Checklist

Before opening a new issue, please verify the following:
1. **Check Existing Issues:** Search the GitHub Issues tab to ensure the bug hasn't already been reported or resolved in a hotfix.
2. **Isolate the Bug:** Can you reproduce the bug reliably using the same steps?
3. **Use the Console Binary (Windows Only):** If you are testing on Windows, please run the game using `game2.console.exe` so you can capture engine stack traces if an unexpected error occurs.

---

## How to Open a Bug Report

When creating a new issue, please use the following template to ensure we have all the telemetry needed to diagnose the root cause.

### 1. Clear Title
Use a descriptive title prefixed with the platform. 
> *Example:* `[Linux] Shader compilation stutter when security cubes explode`

### 2. Environment & System Telemetry
Provide details about your hardware and configuration:
* **OS:** (e.g., Windows 11 Pro 23H2, Ubuntu 22.04 LTS, macOS 14.2)
* **CPU:** (e.g., Intel i5-11400H, AMD Ryzen 5 5600X, Apple M1)
* **GPU & Render Pipeline:** (e.g., NVIDIA GTX 1050 via Vulkan, Intel UHD Graphics via OpenGL 3)
* **System Memory:** Free RAM/VRAM available during the test.

### 3. Steps to Reproduce
List the precise steps to make the bug happen:
1. Launch the game from `[Executable Name]`.
2. Navigate to the main arena loop.
3. Allow the wave count to scale up to X units.
4. Observe the unexpected behavior.

### 4. Expected vs. Actual Behavior
* **Expected:** What the engine *should* do (e.g., "The pause menu opens immediately, capturing mouse input and holding the physics thread").
* **Actual:** What actually happens (e.g., "The pause menu UI renders, but mouse tracking is lost and background elements keep moving").

### 5. Engine Logs & Screenshots
* **Console Logs:** Copy and paste any red execution errors or stack traces printed to the terminal or your `game2.console.exe` window.
* **Media:** Attach screenshots or short video clips showing the visual glitch or performance lag.

---

## Testing Focus Areas for v0.1-alpha1

For this initial release, we are specifically looking for data on:
* **CPU Thread Saturation & Frame Pacing:** Check if Godot’s background asset loading threads choke when the primary game thread is heavily loaded.
* **Window Management & Intercepts:** Ensuring that Alt-Tabbing, minimizing, or clicking out of the viewport bounds triggers the `APPLICATION_FOCUS_OUT` state and pauses the game cleanly.
* **File System Integrity:** Catching any case-sensitivity path breaks or missing resource flags on Linux/macOS filesystems.
* **OS Storage & Workspace Integrity:** Does the game crash silently if it cannot write a local configuration, log file, or cache file to disk? Ensure your graceful scene disconnection and exit sequences leave no orphan temporary data or lockfiles behind in the OS temp directories.

Thank you for keeping *FlashSeek : Grid Combat* bulletproof! Your precise telemetry directly drives our path to a stable Beta.
