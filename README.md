# Making an 8 bit computer

## Design : 
The computer should:
- Use a classic 8bit CPU with a 16bit address space (6502 or Z80)
- Only use DIP packaged, easilly socketable and to solder ICs
- Be able to expose the address and data bus of the CPU to peripheral
- Have a "sniffer/debugger" functionality : Show the state of the bus at any moment
- This means being able to single step the CPU (seems like it's not doable with a 6502 but still possible on a Z80)
- Be a single board computer
- Have a serial interface
- Boot to an "inspector" program that permit to "see" the state of addressed inside the memory space, to write bytes to them directly, and to jump the CPU's program counter to them (to be able to eiter boot an "OS" like Microsoft Basic, or to boot to assembly program writen by the user)
- Have a ZIF socket where the user can put an additional eeprom with arbitrary program data (More or less like game cartrides worked, but simplified down to a single ROM chip)
- Stay easy to wire
- Use modern componant. The processor, ram and rom from the era are still made but in CMOS versions (they are faster and more efficient to use)
- The design should be layed on a board in the same manner a computer architecure diagram would look like. CPU, Buses, ROM, RAM and peripheral clearly labeled
 - The serial interface should be compatibler with a Minitel 1B terminal
 - The board should have a series of control inputs to reset the CPU, stop the clock signal and single step the program.

Usefull links:

 - http://searle.hostei.com/grant/z80/SimpleZ80.html
 - https://en.wikipedia.org/wiki/MAX232
 - https://en.wikipedia.org/wiki/Zilog_Z80

here's a stash of document about the Altair 8800 computer. It uses an intel chip that the z80 is more or less compatible with. Should be a good idea of what's behind the design of a "microcomputer" from the 1970s http://www.classiccmp.org/dunfield/altair/altair6.htm

They still make and sell z80 CPUs https://www.mouser.fr/Semiconductors/Embedded-Processors-Controllers/_/N-6hpef?P=1z0y33f&Keyword=z80&FS=True

