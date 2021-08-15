# Cobalt Strike User-Defined Reflective Loader
Cobalt Strike User-Defined Reflective Loader written in Assembly & C for advanced evasion capabilities.

## Initial Project Goals
+ Cross compile the User-Defined Reflective Loader Cobalt Strike provides with mingw-gcc from macOS/Linux instead of with Windows.
+ Write inline assembly into the project.
+ Have the reflective loader be compatible with Cobalt Strike via the API functionality and kit provided in the new update.
+ Learn how reflective loader works.
+ Write my own reflective loader in assembly.

## Future Project Goals
+ Use the initial project as a template for more advanced evasion techniques leveraging the evasion flexibility of Assembly.
+ Implement the Cobalt Strike options such as no RWX, stompPE, module stomping, changing the MZ header, etc.
+ Write a decent Aggressor script.
+ Have different versions of reflective loader to choose from.
+ Implement HellsGate/HalosGate for the initial calls that reflective loader uses (NtFlushCache,VirtualAlloc,GetProcAddress,LoadLibraryA,etc)
+ Optimize the assembly code.
+ Some kind of template language overlay that can modify/randomize the registers/methods.

## Credits / References
### Reflective Loader
+ https://github.com/stephenfewer/ReflectiveDLLInjection
+ https://institute.sektor7.net/courses/rto-maldev-intermediate/463258-reflective-dlls
### Cobalt Strike User Defined Reflective Loader
+ https://www.cobaltstrike.com/help-user-defined-reflective-loader
### Implementing ASM in C Code with GCC
+ https://outflank.nl/blog/2020/12/26/direct-syscalls-in-beacon-object-files/
+ https://www.cs.uaf.edu/2011/fall/cs301/lecture/10_12_asm_c.html