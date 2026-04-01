# uhhhhhh

## In-Browser x86 Virtual Machine

This project provides a simple web-based x86 virtual machine emulator that runs entirely in the browser.

### Features
- 2048 MB RAM
- 128 MB Video Memory
- Upload and boot from .iso files
- Default terminal/kernel boot for basic content management (if no ISO selected)
- noVNC client for connecting to VNC servers (if the VM OS has one running on localhost:5900)
- No external server required - everything runs client-side

### Usage
1. Open `index.html` in a modern web browser (Chrome, Firefox, etc.)
2. Optionally, click "Choose File" and select a .iso file
3. Click "Start VM" to boot the virtual machine
   - If no ISO: Boots to a default Linux kernel with serial terminal for basic commands
   - If ISO: Boots the ISO with graphical display
4. Interact with the VM using your keyboard and mouse
5. For content management in terminal mode: Use the serial terminal interface
6. For graphical content management: If your ISO includes a VNC server, use "Connect to VNC" button
7. Click "Stop VM" to halt the emulator

### Requirements
- Modern web browser with WebAssembly support
- Sufficient system RAM (the emulator uses ~2GB)

### Notes
- Performance depends on your system's capabilities
- Large ISOs may take time to load
- Keyboard input is supported; mouse is captured when clicking on the screen
- noVNC connection requires the VM to have a VNC server running and accessible (not possible in pure browser environment without external setup)
- Default terminal provides basic shell access for content management