# llvm-mc-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: llvm machine code playground

USAGE: llvm-mc-3.6 [options] <input file>

OPTIONS:
  -I=<directory>                                  - Directory of include files
  -aarch64-neon-syntax                            - Choose style of NEON code to emit from AArch64 backend:
    =generic                                      -   Emit generic NEON assembly
    =apple                                        -   Emit Apple-style NEON assembly
  -arch=<string>                                  - Target arch to assemble for, see -version for available targets
  -asm-instrumentation                            - Instrumentation of inline assembly and assembly source files
    =none                                         -   no instrumentation at all
    =address                                      -   instrument instructions with memory arguments
  -asm-show-inst                                  - Emit internal instruction representation to assembly file
  -bounds-checking-single-trap                    - Use one trap block per function
  -code-model                                     - Choose code model
    =default                                      -   Target default code model
    =small                                        -   Small code model
    =kernel                                       -   Kernel code model
    =medium                                       -   Medium code model
    =large                                        -   Large code model
  -color                                          - use colored syntax highlighting (default=autodetect)
  -compress-debug-sections                        - Compress DWARF debug sections
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
  -disable-spill-fusing                           - Disable fusing of spill code into instructions
  -dwarf-version=<int>                            - Dwarf version
  -enable-load-pre                                - 
  -enable-misched                                 - Enable the machine instruction scheduling pass.
  -enable-objc-arc-opts                           - enable/disable all ARC Optimizations
  -enable-scoped-noalias                          - 
  -enable-tbaa                                    - 
  -exhaustive-register-search                     - Exhaustive Search for registers bypassing the depth and interference cutoffs of last chance recoloring
  -fdebug-compilation-dir=<string>                - Specifies the debug info's compilation dir
  -filetype                                       - Choose an output file type:
    =asm                                          -   Emit an assembly ('.s') file
    =null                                         -   Don't emit anything (for timing purposes)
    =obj                                          -   Emit a native object ('.o') file
  -g                                              - Generate dwarf debugging info for assembly source files
  -help                                           - Display available options (-help-hidden for more)
  -internalize-public-api-file=<filename>         - A file containing list of symbol names to preserve
  -internalize-public-api-list=<list>             - A list of symbol names to preserve
  -join-liveintervals                             - Coalesce copies (default=true)
  -limit-float-precision=<uint>                   - Generate low-precision inline sequences for some float libcalls
  -main-file-name=<string>                        - Specifies the name we should consider the input file
  -mattr=<a1,+a2,-a3,...>                         - Target specific attributes (-mattr=help for details)
  -mc-relax-all                                   - When used with filetype=obj, relax all fixups in the emitted object file
  -mc-x86-disable-arith-relaxation                - Disable relaxation of arithmetic instruction for X86
  -mcpu=<cpu-name>                                - Target a specific cpu type (-mcpu=help for details)
  Action to perform:
    -as-lex                                       - Lex tokens from a .s file
    -assemble                                     - Assemble a .s file (default)
    -disassemble                                  - Disassemble strings of hex bytes
    -mdis                                         - Marked up disassembly of strings of hex bytes
  -mips16-constant-islands                        - MIPS: mips16 constant islands enable.
  -mips16-hard-float                              - MIPS: mips16 hard float enable.
  -mno-ldc1-sdc1                                  - Expand double precision loads and stores to their single precision counterparts
  -n                                              - Don't assume assembly file starts in the text section
  -no-discriminators                              - Disable generation of discriminator information.
  -no-exec-stack                                  - File doesn't need an exec stack
  -nvptx-sched4reg                                - NVPTX Specific: schedule for register pressue
  -o=<filename>                                   - Output filename
  -output-asm-variant=<uint>                      - Syntax variant to use for output printing
  -print-after-all                                - Print IR after each pass
  -print-before-all                               - Print IR before each pass
  -print-imm-hex                                  - Prefer hex format for immediate values
  -print-machineinstrs=<pass-name>                - Print machine instrs
  -regalloc                                       - Register allocator to use
    =default                                      -   pick register allocator based on -O option
    =basic                                        -   basic register allocator
    =fast                                         -   fast register allocator
    =greedy                                       -   greedy register allocator
    =pbqp                                         -   PBQP register allocator
  -relocation-model                               - Choose relocation model
    =default                                      -   Target default relocation model
    =static                                       -   Non-relocatable code
    =pic                                          -   Fully relocatable, position independent code
    =dynamic-no-pic                               -   Relocatable external references, non-relocatable code
  -rewrite-map-file=<filename>                    - Symbol Rewrite Map
  -rng-seed=<seed>                                - Seed for the random number generator
  -sample-profile-max-propagate-iterations=<uint> - Maximum number of iterations to go through when propagating sample block/edge weights through the CFG.
  -save-temp-labels                               - Don't discard temporary labels
  -show-encoding                                  - Show instruction encodings
  -show-inst                                      - Show internal instruction representation
  -show-inst-operands                             - Show instructions operands as parsed
  -stackmap-version=<int>                         - Specify the stackmap encoding version (default = 1)
  -stats                                          - Enable statistics output from program (available with Asserts)
  -time-passes                                    - Time each pass, printing elapsed time for each on exit
  -triple=<string>                                - Target triple to assemble for, see -version for available targets
  -verify-debug-info                              - 
  -verify-dom-info                                - Verify dominator info (time consuming)
  -verify-loop-info                               - Verify loop info (time consuming)
  -verify-regalloc                                - Verify during register allocation
  -verify-region-info                             - Verify region info (time consuming)
  -verify-scev                                    - Verify ScalarEvolution's backedge taken counts (slow)
  -version                                        - Display the version of this program
  -x86-asm-syntax                                 - Choose style of code to emit from X86 backend:
    =att                                          -   Emit AT&T-style assembly
    =intel                                        -   Emit Intel-style assembly
  -x86-recip-refinement-steps=<int>               - Specify the number of Newton-Raphson iterations applied to the result of the hardware reciprocal estimate instruction.

~~~
