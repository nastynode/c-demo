# Simple C program
C++ is built on C, so any C program can be compiled with the C++ compiler. Since this program doesn't need any of the additional functionality of C++, I gave it the `.c` extension and used my C compiler. You could use the C++ compiler, and/or change the extension to `.cpp` and it wouldn't make a difference. You can use any C code or C library in a C++ program (but not the other way around).

# Makefiles
Makefiles are kind of like scripts for compiling or running your program with default settings. This is helpful when you notice youself running the same commands (or series of commands) repeatedly. These are especially helpful when you start adding in external C++ libraries or you want to compile your program with different warnings enabled/disabled.

In the sample Makefile, `make` will compile the program with gcc (global c compiler). Depending on what compiler you have on your machine, you may need to change this. Try changing the makefile to use your C++ compiler and see what happens!

`make clean` will clean up any compiled binaries, and will need to be run before you can run `make` again. `make run` will run the compiled program with some sample arguments