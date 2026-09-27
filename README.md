# Reverse Engineering Walkthroughs 🐛

This repository contains my personal notes, write-ups, and walkthroughs on binary analysis and reverse engineering.

## 1. Basic Binary Patching 
**Objective:** To analyze and patch a basic executable file to bypass a simple check.
**Tools Used:** Kali Linux, OllyDbg / x64dbg

### Process:
1. **Initial Analysis:** Opened the binary in OllyDbg and analyzed the execution flow.
2. **Finding the Logic:** Located the conditional jump instruction (e.g., `JNZ` or `JE`) responsible for the access validation.
3. **Patching the Binary:** Modified the instruction to bypass the logic (e.g., changing `JNZ` to `NOP` instructions).
4. **Result:** The application flow was successfully redirected.
