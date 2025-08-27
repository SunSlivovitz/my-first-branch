# Presentación
<img src="https://i.pinimg.com/736x/b1/52/71/b15271f5f719a6386d72904fe6c04b35.jpg" alt="Jem and The Holograms" width="200">

*Hola! mi nombre es Juana.*

*En mi tiempo libre me gusta diseñar websites con estilo de los 90's y 2000's.*  
*Mi instrucción favorita del manual de Intel es mov. David la explicó con mucha onda.*

## Cositas de Intel
### Saving and Restoring the SSE/SSE2 State
>The `FXSAVE` instruction saves the x87 FPU, MMX, SSE, and SSE2 states (which includes the contents of eight XMM registers and the MXCSR registers) in a 512-byte block of memory. The `FXRSTOR` instruction restores the saved SSE and SSE2 state from memory. See the `FXSAVE` instruction in Chapter 3 of the Intel® 64 and IA-32 Architectures Software Developer’s Manual, Volume 2A, for the layout of the 512-byte state block.
>
>In addition to saving and restoring the SSE and SSE2 state, `FXSAVE` and `FXRSTOR` also save and restore the x87 FPU state (because MMX registers are aliased to the x87 FPU data registers this includes saving and restoring the MMX state). For greater code efficiency, it is suggested that `FXSAVE` and `FXRSTOR` be substituted for the FSAVE, FNSAVE, and FRSTOR instructions in the following situations:
> - When a context switch is being made in a multitasking environment
> - During calls and returns from interrupt and exception handlers
>
>In situations where the code is switching between x87 FPU and MMX technology computations (without a context switch or a call to an interrupt or exception), the FSAVE/FNSAVE and FRSTOR instructions are more efficient than the FXSAVE and FXRSTOR instructions.

Pág. 290 del manual <a href="https://www.intel.la/content/www/xl/es/content-details/782158/intel-64-and-ia-32-architectures-software-developer-s-manual-combined-volumes-1-2a-2b-2c-2d-3a-3b-3c-3d-and-4.html" target="_blank">"Intel® 64 and IA-32 Architectures Software Developer"</a>.</p>
