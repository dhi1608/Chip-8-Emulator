Chip-8 Emulator

Create a CPU emulator for the Chip-8 processor. The Chip-8 is a processor from the 70's that is an excellent introduction to hardware emulation as it has a limited instruction set and is very well documented. Writing the emulator from scratch will give you some very good exposure to the type of software we deal with. Here is a decent sequence of events...

1. Research Chip-8; gather data sheets / instruction set info; gather some sample Chip-8 ROMs.
2. Create a disassembler and make sure it produces sensible output for a known good ROM.
3. Emulate the CPU (i.e. handle sequences of opcodes with your virtual processor).
4. Emulate the peripheral devices like user input, sound / video output. This part is less important, so feel free to cheat on this part from existing code on the internet.

Requirements:

1. The emulator shall be capable of disassembling a Chip-8 ROM and producing source assembly listings.
2. The emulator shall be capable of executing a Chip-8 ROM without crashing.
3. The emulator shall be able to accept user input via keyboard and produce a graphical display.

Building:

The development environment for this application is Windows10 OS utilizing Mingw-w64 GCC compiler for windows, SDL2 libraries and Git Bash.  As a result, the makefile environment is configured based on Mingw-w64 and executes in a Git Bash environment which is the equivalent of an xterm for Windows.  

This project consists of two executable binary files: ChipDecoder.exe and Chip8.exe.  These files can be generated by executing the default make command in the src directory.

Running applications from bin directory:

Decoder - this application disassembles a Chip-8 ROM and produces assembly.

./Chip8Decoder.exe ../roms/(filename)
  
Emulator - this application executes a Chip-8 ROM

./Chip8.exe ../roms/(filename)
