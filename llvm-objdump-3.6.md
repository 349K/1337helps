# llvm-objdump-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: llvm object file dumper

USAGE: llvm-objdump-3.6 [options] <input object files>

OPTIONS:
  -aarch64-neon-syntax                            - Choose style of NEON code to emit from AArch64 backend:
    =generic                                      -   Emit generic NEON assembly
    =apple                                        -   Emit Apple-style NEON assembly
  -arch=<string>                                  - architecture(s) from a Mach-O file to dump
  -arch-name=<string>                             - Target arch to disassemble for, see -version for available targets
  -bind                                           - Display mach-o binding info
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
  -disable-spill-fusing                           - Disable fusing of spill code into instructions
  -disassemble                                    - Display assembler mnemonics for the machine instructions
  -dsym=<string>                                  - Use .dSYM file for debug info
  -enable-load-pre                                - 
  -enable-misched                                 - Enable the machine instruction scheduling pass.
  -enable-objc-arc-opts                           - enable/disable all ARC Optimizations
  -enable-scoped-noalias                          - 
  -enable-tbaa                                    - 
  -exhaustive-register-search                     - Exhaustive Search for registers bypassing the depth and interference cutoffs of last chance recoloring
  -exports-trie                                   - Display mach-o exported symbols
  -full-leading-addr                              - Print full leading address
  -g                                              - Print line information from debug info if available
  -help                                           - Display available options (-help-hidden for more)
  -internalize-public-api-file=<filename>         - A file containing list of symbol names to preserve
  -internalize-public-api-list=<list>             - A list of symbol names to preserve
  -join-liveintervals                             - Coalesce copies (default=true)
  -lazy-bind                                      - Display mach-o lazy binding info
  -limit-float-precision=<uint>                   - Generate low-precision inline sequences for some float libcalls
  -macho                                          - Use MachO specific object file parser
  -mattr=<a1,+a2,-a3,...>                         - Target specific attributes
  -mc-x86-disable-arith-relaxation                - Disable relaxation of arithmetic instruction for X86
  -mcpu=<cpu-name>                                - Target a specific cpu type (-mcpu=help for details)
  -mips16-constant-islands                        - MIPS: mips16 constant islands enable.
  -mips16-hard-float                              - MIPS: mips16 hard float enable.
  -mno-ldc1-sdc1                                  - Expand double precision loads and stores to their single precision counterparts
  -no-discriminators                              - Disable generation of discriminator information.
  -no-show-raw-insn                               - When disassembling instructions, do not print the instruction bytes.
  -nvptx-sched4reg                                - NVPTX Specific: schedule for register pressue
  -print-after-all                                - Print IR after each pass
  -print-before-all                               - Print IR before each pass
  -print-imm-hex                                  - Use hex format for immediate values
  -print-machineinstrs=<pass-name>                - Print machine instrs
  -private-headers                                - Display format specific file headers
  -r                                              - Display the relocation entries in the file
  -rebase                                         - Display mach-o rebasing info
  -regalloc                                       - Register allocator to use
    =default                                      -   pick register allocator based on -O option
    =basic                                        -   basic register allocator
    =fast                                         -   fast register allocator
    =greedy                                       -   greedy register allocator
    =pbqp                                         -   PBQP register allocator
  -rewrite-map-file=<filename>                    - Symbol Rewrite Map
  -rng-seed=<seed>                                - Seed for the random number generator
  -s                                              - Display the content of each section
  -sample-profile-max-propagate-iterations=<uint> - Maximum number of iterations to go through when propagating sample block/edge weights through the CFG.
  -section-headers                                - Display summaries of the headers for each section.
  -stackmap-version=<int>                         - Specify the stackmap encoding version (default = 1)
  -stats                                          - Enable statistics output from program (available with Asserts)
  -t                                              - Display the symbol table
  -time-passes                                    - Time each pass, printing elapsed time for each on exit
  -triple=<string>                                - Target triple to disassemble for, see -version for available targets
  -universal-headers                              - Print Mach-O universal headers
  -unwind-info                                    - Display unwind information
  -verify-debug-info                              - 
  -verify-dom-info                                - Verify dominator info (time consuming)
  -verify-loop-info                               - Verify loop info (time consuming)
  -verify-regalloc                                - Verify during register allocation
  -verify-region-info                             - Verify region info (time consuming)
  -verify-scev                                    - Verify ScalarEvolution's backedge taken counts (slow)
  -version                                        - Display the version of this program
  -weak-bind                                      - Display mach-o weak binding info
  -x86-asm-syntax                                 - Choose style of code to emit from X86 backend:
    =att                                          -   Emit AT&T-style assembly
    =intel                                        -   Emit Intel-style assembly
  -x86-recip-refinement-steps=<int>               - Specify the number of Newton-Raphson iterations applied to the result of the hardware reciprocal estimate instruction.

~~~
