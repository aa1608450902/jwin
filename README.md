# jwin
For learning Windows programming.

### Windows Program Learning Steps

---

- Basic win32 windows invoking API framework
- Learn to use compile resource by using resource script(provided by VC++6.0)
- Learn how to use GDI to design UI components
- Learn the basic MFC framework # not very important
- Basic operation # (file operation and dll, hook)
- Winsock programming # the basic processes
- Kernel service programming and system call api design # very important
- Design of opengl program # be associated with game programming

### Constitution Of Win32 SDK

---

#### lib/dll
- kernel32.dll # provided the core API of thread, process, memory management ... 
- user32.dll   # provided the API of window, message
- gdi32.dll    # provided the API of draw

#### header
- windef.h 	# the data type of windows
- winbase.h # include all declaration of kernel32.dll API
- wingdi.h 	# include all declaration of gdi32.dll API
- winuser.h # include all declaration of user32.dll API
- winnt.h 	# include the support of UNICODE char collection
- windows.h # the collection of all windows header files

### Special Keywords

---

- eg. [__stdcall]
- eg. [__declspec]
- eg. [__restrict]
- eg. 

### Precompiler

---

#### The basic precompiler command
- eg. #define #undef #include
- eg. #define __ID(s) ID##s // Splicing identifier
- eg. #define DECLARE_HANDLE(name) struct name##__ { int unused; }; typedef struct name##__ *name
- eg. #error // force to stop compiling
- eg. #if #else #elif #endif
- eg. #if defined(...) // = #ifdef ...
- eg. #line
- eg. #pragma message("...")
- eg. #pragma code_seg(["section-name"[,"section-class"] ])
- eg. #pragma once
- eg. #pragma hdrstop
- eg. #pragma resource "*.dfm" // put *.dfm resource file into project
- eg. #pragma warning( disable : 4507 34; once : 4385; error : 164 )
- eg. #pragma comment(...)
- eg. #progma pack(n)

#### The advanced usage
- typedef char TCHAR, *PTCHAR; // = typedef char TCHAR; typedef char * PTCHAR;
- eg. #ifdef __cplusplus; extern "C" {; #endif; #ifdef __cplusplus; }; #endif;
- eg. 

### The Key Of Win32 Program

---

- Differences between Win32 CONSOLE program and Win32 Windows program - Link options (SUBSYSTEM:CONSOLE) / (SUBSYSTEM:WINDOWS)
- The specialized keyword in Windows Operation System - __stdcall/__cdecl/_clrcall/__fastcall/__thiscall/__vectorcall
- Conception - Kernel Object
- DLL And Hook Tech in Windows OS
- Microsoft Platform SDK (Software Development Kit) - for VC # This importance, you must treat .h & .lib as the SDK of Windows OS development.
- Windows system programming [reference](https://msdn.microsoft.com/zh-cn)

### The Shortcuts In Visual Studio

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
- rc.exe - Resource compiler

### ABI In Windows

---

- Try to parse PE file structure - What is PE loader?
- Constitution of ABI in Windows OS
- Relationship between compiler and linker - OS implemented the ABI by using compiler and linker.

### Git

---

- git add [ file ]
- git commit -m "update message"
- git push origin [ branch ]