# jwin
For learning Windows programming.

### windows program learning steps

---

- basic win32 windows invoking API framework
- learn to use compile resource by using resource script(provided by VC++6.0)
- learn how to use GDI to design UI components
- learn the basic MFC framework # not very important
- basic operation # (file operation and dll, hook)
- winsock programming # the basic processes
- kernel service programming and system call api design # very important
- design of opengl program # be associated with game programming

### The Key Of Win32 Program

---

- Differences between Win32 CONSOLE program and Win32 Windows program - Link options (SUBSYSTEM:CONSOLE) / (SUBSYSTEM:WINDOWS)
- The specialized keyword in Windows Operation System - __stdcall/__cdecl/_clrcall/__fastcall/__thiscall/__vectorcall
- Conception - Kernel Object
- DLL And Hook Tech in Windows OS
- Microsoft Platform SDK (Software Development Kit) - for VC # This importance, you must treat .h & .lib as the SDK of Windows OS development.
- Windows system programming [reference](https://msdn.microsoft.com/zh-cn)

### The shortcuts in Visual Studio

---

- ctrl + j - code hinting
- ctrl + shift + b - Generating solution
- ctrl + shift + c - Open class viewer
- ctrl + shift + e - Open resource viewer
- ctrl + alt + l - Open explorer
- ctrl + - - The cursor/navigation back
- F12 - To definition

### Compile Tools In Windows

---

- cl.exe - Microsoft C/C++ Compiler # You must know the common compiler options.
- nmake.exe - makefile
- link.exe - Linker options

### ABI In Windows

---

- Try to parse PE file structure - What is PE loader?
- Constitution of ABI in Windows OS
- Relationship between compiler and linker - OS implemented the ABI by using compiler and linker.
