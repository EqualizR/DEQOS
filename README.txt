Hey guys

this is version 0.9 of DEQOS, a fully functionnal operating system for DCPU-16
here are the key features (actually working right now) :

- Real Preemptive multi tasking (with priorities and everything...)
- Multi consoles (3 linux-like virtual consoles, with instant switch using CTRL+1,2 or 3)
- Semaphore synchronization (mutex, focus-sync)
- Memory allocation (malloc, free)
- Tiny FAT system (whole FAT in one sector for faster response)
- Boot loader : loads the system from disk
- Program loading and executing using the LOADP NAME.PRG command
- Client programs API (Stack, Gui, Keyboard, Memory, Time, Disk, 32 bit Math, etc...), all thread safe
- Supports the NE_LEM1802 screen, HIT_HMD2043 disk drive, Generic Clock and Generic Keyboard devices

Source code is available, customize it, port it, contribute,
or just use the code as a reference as you wish (please credit me somewhere if you do ;) )
Code is heavily commented and *MAY* help some beginners to understand how Operating System works
(especially on the multi threading / Mutex parts)

.. and have fun with it :)

DEQOS can be tested using the provided "DCPUStation" Assembler/Emulator/Symbolic debugger (Windows/Linux (with mono) ).
Several sample programs have been included in the test project.
To test, launch DCPUStation.exe (on Linux, type "mono DCPUStation.exe" in a terminal)
then open the DEQOS_Project.vdcpu16 project, and select Build/Assemble and Run
Then, use CTRL-1 CTRL-2 and CTRL-3 to alternate between virtual consoles
commands are : DIR to list the files on the disk, LOADP to run programs, MEM to show the available memory



PS, in the works : DOS-like text drop down menus and windows, Text editor.

EqualizR
equalizr@free.fr
