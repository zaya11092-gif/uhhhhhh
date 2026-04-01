# uhhhhhh

## In-Browser x86 Virtual Machine

This project provides a simple web-based x86 virtual machine emulator that runs entirely in the browser.

### Features
- 2048 MB RAM
- 128 MB Video Memory
- Upload and boot from .iso files
- No external server required - everything runs client-side

### Usage
1. Open `index.html` in a modern web browser (Chrome, Firefox, etc.)
2. Click "Choose File" and select a .iso file
3. Click "Start VM" to boot the virtual machine
4. Interact with the VM using your keyboard and mouse
5. Click "Stop VM" to halt the emulator

### Requirements
- Modern web browser with WebAssembly support
- Sufficient system RAM (the emulator uses ~2GB)

### Notes
- Performance depends on your system's capabilities
- Large ISOs may take time to load
- Keyboard input is supported; mouse is captured when clicking on the screen