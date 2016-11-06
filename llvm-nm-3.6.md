# llvm-nm-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: llvm symbol table dumper

USAGE: llvm-nm-3.6 [options] <input files> --s Dump only symbols from this segment and section name, Mach-O only

OPTIONS:
  -B                                              - Alias for --format=bsd
  -P                                              - Alias for --format=posix
  -aarch64-neon-syntax                            - Choose style of NEON code to emit from AArch64 backend:
    =generic                                      -   Emit generic NEON assembly
    =apple                                        -   Emit Apple-style NEON assembly
  -arch=<string>                                  - architecture(s) from a Mach-O file to dump
  -bounds-checking-single-trap                    - Use one trap block per function
  -color                                          - use colored syntax highlighting (default=autodetect)
  -cppfname=<function name>                       - Specify the name of the generated function
  -cppfor=<string>                                - Specify the name of the thing to generate
  -cppgen                                         - Choose what kind of output to generate
    =program                                      -   Generate a complete program
    =module                                       -   Generate a module definition
    =contents                                     -   Generate contents of a module
    =function                                     -   Generate a function definition
    =functions                                    -   Generate all function definitions
    =inline                                       -   Generate an inline function
    =variable                                     -   Generate a variable definition
    =type                                         -   Generate a type definition
  -debug-syms                                     - Show all symbols, even debugger only
  -defined-only                                   - Show only defined symbols
  -disable-spill-fusing                           - Disable fusing of spill code into instructions
  -dynamic                                        - Display the dynamic symbols instead of normal symbols.
  -enable-load-pre                                - 
  -enable-misched                                 - Enable the machine instruction scheduling pass.
  -enable-objc-arc-opts                           - enable/disable all ARC Optimizations
  -enable-scoped-noalias                          - 
  -enable-tbaa                                    - 
  -exhaustive-register-search                     - Exhaustive Search for registers bypassing the depth and interference cutoffs of last chance recoloring
  -extern-only                                    - Show only external symbols
  -format                                         - Specify output format
    =bsd                                          -   BSD format
    =sysv                                         -   System V format
    =posix                                        -   POSIX.2 format
    =darwin                                       -   Darwin -m format
  -help                                           - Display available options (-help-hidden for more)
  -internalize-public-api-file=<filename>         - A file containing list of symbol names to preserve
  -internalize-public-api-list=<list>             - A list of symbol names to preserve
  -join-liveintervals                             - Coalesce copies (default=true)
  -just-symbol-name                               - Print just the symbol's name
  -limit-float-precision=<uint>                   - Generate low-precision inline sequences for some float libcalls
  -m                                              - Alias for --format=darwin
  -mc-x86-disable-arith-relaxation                - Disable relaxation of arithmetic instruction for X86
  -mips16-constant-islands                        - MIPS: mips16 constant islands enable.
  -mips16-hard-float                              - MIPS: mips16 hard float enable.
  -mno-ldc1-sdc1                                  - Expand double precision loads and stores to their single precision counterparts
  -no-discriminators                              - Disable generation of discriminator information.
  -no-llvm-bc                                     - Disable LLVM bitcode reader
  -no-sort                                        - Show symbols in order encountered
  -numeric-sort                                   - Sort symbols by address
  -nvptx-sched4reg                                - NVPTX Specific: schedule for register pressue
  -print-after-all                                - Print IR after each pass
  -print-armap                                    - Print the archive map
  -print-before-all                               - Print IR before each pass
  -print-file-name                                - Precede each symbol with the object file it came from
  -print-machineinstrs=<pass-name>                - Print machine instrs
  -print-size                                     - Show symbol size instead of address
  -regalloc                                       - Register allocator to use
    =default                                      -   pick register allocator based on -O option
    =basic                                        -   basic register allocator
    =fast                                         -   fast register allocator
    =greedy                                       -   greedy register allocator
    =pbqp                                         -   PBQP register allocator
  -reverse-sort                                   - Sort in reverse order
  -rewrite-map-file=<filename>                    - Symbol Rewrite Map
  -rng-seed=<seed>                                - Seed for the random number generator
  -s=<string>                                     - Dump only symbols from this segment and section name, Mach-O only
  -sample-profile-max-propagate-iterations=<uint> - Maximum number of iterations to go through when propagating sample block/edge weights through the CFG.
  -size-sort                                      - Sort symbols by size
  -stackmap-version=<int>                         - Specify the stackmap encoding version (default = 1)
  -stats                                          - Enable statistics output from program (available with Asserts)
  -time-passes                                    - Time each pass, printing elapsed time for each on exit
  -undefined-only                                 - Show only undefined symbols
  -verify-debug-info                              - 
  -verify-dom-info                                - Verify dominator info (time consuming)
  -verify-loop-info                               - Verify loop info (time consuming)
  -verify-regalloc                                - Verify during register allocation
  -verify-region-info                             - Verify region info (time consuming)
  -verify-scev                                    - Verify ScalarEvolution's backedge taken counts (slow)
  -version                                        - Display the version of this program
  -x                                              - Print symbol entry in hex, Mach-O only
  -x86-asm-syntax                                 - Choose style of code to emit from X86 backend:
    =att                                          -   Emit AT&T-style assembly
    =intel                                        -   Emit Intel-style assembly
  -x86-recip-refinement-steps=<int>               - Specify the number of Newton-Raphson iterations applied to the result of the hardware reciprocal estimate instruction.

~~~
