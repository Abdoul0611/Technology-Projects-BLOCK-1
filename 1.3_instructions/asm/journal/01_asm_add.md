# Checkpoint 1 -asm add

#Which registers are used and why?#
Only r0 is used .mov r0, #5 puts the number into r0, then add r0, r0, #3 adds 3 to the value already in r0, so r0, ends up as 8.
r0 is just ht genreal purpose register that I used to hold thge numbe.

One observation is that nothing is printed on screen. The result (8) olny can be found inside the r0 register. At the end, there is a segementation fault because no exit instruction was added, so the the CPU carries on past the end
of my code.
## Snippet from add.disasm.txt
 400078:	d28000a0 	mov	x0, #0x5                   	// #5
  400080:	d2800ba8 	mov	x8, #0x5d                  	// #93

