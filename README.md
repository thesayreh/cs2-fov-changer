📌 cs2-fov-changer
Description
cs2-fov-changer is a lightweight C++ tool that modifies the Field of View (FOV) value in Counter-Strike 2 by accessing and writing to the game's process memory. It demonstrates fundamental memory manipulation techniques using the Windows API.

🔧 Features
Locates the running Counter-Strike 2 window using its title.

Retrieves the process ID and opens it with full access rights.

Scans the process's loaded modules to find the base address of client.dll.

Reads a known offset (0x1A459E0) to obtain a pointer to the player data structure.

Writes a new FOV value (120) to the correct memory address at offset +0x6F4.

🛠️ Technologies Used
WinAPI: FindWindow, GetWindowThreadProcessId, OpenProcess, ReadProcessMemory, WriteProcessMemory

Module scanning: CreateToolhelp32Snapshot, Module32First, Module32Next

Low-level memory manipulation and reverse-engineering concepts

⚠️ Disclaimer
This project is for educational and research purposes only. It is intended to demonstrate how memory interaction works in Windows and should not be used to gain unfair advantage in online games.

