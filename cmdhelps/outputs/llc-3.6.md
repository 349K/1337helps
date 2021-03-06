# llc-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: llvm system compiler

USAGE: llc-3.6 [options] <input bitcode>

OPTIONS:
  -O=<char>                                       - Optimization level. [-O0, -O1, -O2, or -O3] (default = '-O2')
  -aarch64-neon-syntax                            - Choose style of NEON code to emit from AArch64 backend:
    =generic                                      -   Emit generic NEON assembly
    =apple                                        -   Emit Apple-style NEON assembly
  -asm-instrumentation                            - Instrumentation of inline assembly and assembly source files
    =none                                         -   no instrumentation at all
    =address                                      -   instrument instructions with memory arguments
  -asm-show-inst                                  - Emit internal instruction representation to assembly file
  -asm-verbose                                    - Add comments to directives.
  -bounds-checking-single-trap                    - Use one trap block per function
  -cfi-enforcing                                  - Enforce CFI or pass the violation to a function.
  -cfi-func-name=<string>                         - The name of the CFI function to call
  -cfi-type                                       - Choose the type of Control-Flow Integrity check to add
    =sub                                          -   Subtract the pointer from the table base, then mask.
    =ror                                          -   Use rotate to check the offset from a table base.
    =add                                          -   Mask out the high bits and add to an aligned base.
  -code-model                                     - Choose code model
    =default                                      -   Target default code model
    =small                                        -   Small code model
    =kernel                                       -   Kernel code model
    =medium                                       -   Medium code model
    =large                                        -   Large code model
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
  -data-sections                                  - Emit data into separate sections
  -disable-fp-elim                                - Disable frame pointer elimination optimization
  -disable-simplify-libcalls                      - Disable simplify-libcalls
  -disable-spill-fusing                           - Disable fusing of spill code into instructions
  -disable-tail-calls                             - Never emit tail calls
  -dwarf-version=<int>                            - Dwarf version
  -enable-fp-mad                                  - Enable less precise MAD instructions to be generated
  -enable-load-pre                                - 
  -enable-misched                                 - Enable the machine instruction scheduling pass.
  -enable-no-infs-fp-math                         - Enable FP math optimizations that assume no +-Infs
  -enable-no-nans-fp-math                         - Enable FP math optimizations that assume no NaNs
  -enable-objc-arc-opts                           - enable/disable all ARC Optimizations
  -enable-pie                                     - Assume the creation of a position independent executable.
  -enable-scoped-noalias                          - 
  -enable-tbaa                                    - 
  -enable-unsafe-fp-math                          - Enable optimizations that may decrease FP precision
  -exhaustive-register-search                     - Exhaustive Search for registers bypassing the depth and interference cutoffs of last chance recoloring
  -fcfi                                           - Apply forward-edge control-flow integrity
  -filetype                                       - Choose a file type (not all types are supported by all targets):
    =asm                                          -   Emit an assembly ('.s') file
    =obj                                          -   Emit a native object ('.o') file
    =null                                         -   Emit nothing, for performance testing
  -float-abi                                      - Choose float ABI type
    =default                                      -   Target default float ABI type
    =soft                                         -   Soft float ABI (implied by -soft-float)
    =hard                                         -   Hard float ABI (uses FP registers)
  -fp-contract                                    - Enable aggressive formation of fused FP ops
    =fast                                         -   Fuse FP ops whenever profitable
    =on                                           -   Only fuse 'blessed' FP ops.
    =off                                          -   Only fuse FP ops when the result won't be effected.
  -function-sections                              - Emit functions into separate sections
  -help                                           - Display available options (-help-hidden for more)
  -internalize-public-api-file=<filename>         - A file containing list of symbol names to preserve
  -internalize-public-api-list=<list>             - A list of symbol names to preserve
  -join-liveintervals                             - Coalesce copies (default=true)
  -jump-table-type                                - Choose the type of Jump-Instruction Table for jumptable.
    =single                                       -   Create a single table for all jumptable functions
    =arity                                        -   Create one table per number of parameters.
    =simplified                                   -   Create one table per simplified function type.
    =full                                         -   Create one table per unique function type.
  -limit-float-precision=<uint>                   - Generate low-precision inline sequences for some float libcalls
  -load=<pluginfilename>                          - Load the specified plugin
  -march=<string>                                 - Architecture to generate code for (see --version)
  -mattr=<a1,+a2,-a3,...>                         - Target specific attributes (-mattr=help for details)
  -mc-relax-all                                   - When used with filetype=obj, relax all fixups in the emitted object file
  -mc-x86-disable-arith-relaxation                - Disable relaxation of arithmetic instruction for X86
  -mcpu=<cpu-name>                                - Target a specific cpu type (-mcpu=help for details)
  -mips16-constant-islands                        - MIPS: mips16 constant islands enable.
  -mips16-hard-float                              - MIPS: mips16 hard float enable.
  -mno-ldc1-sdc1                                  - Expand double precision loads and stores to their single precision counterparts
  -mtriple=<string>                               - Override target triple for module
  -no-discriminators                              - Disable generation of discriminator information.
  -nozero-initialized-in-bss                      - Don't place zero-initialized symbols into bss section
  -nvptx-sched4reg                                - NVPTX Specific: schedule for register pressue
  -o=<filename>                                   - Output filename
  -print-after-all                                - Print IR after each pass
  -print-before-all                               - Print IR before each pass
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
  -soft-float                                     - Generate software floating point library calls
  -stack-alignment=<uint>                         - Override default stack alignment
  -stackmap-version=<int>                         - Specify the stackmap encoding version (default = 1)
  -start-after=<pass-name>                        - Resume compilation after a specific pass
  -stats                                          - Enable statistics output from program (available with Asserts)
  -stop-after=<pass-name>                         - Stop compilation after a specific pass
  -tailcallopt                                    - Turn fastcc calls into tail calls by (potentially) changing ABI.
  -thread-model                                   - Choose threading model
    =posix                                        -   POSIX thread model
    =single                                       -   Single thread model
  -time-passes                                    - Time each pass, printing elapsed time for each on exit
  -use-ctors                                      - Use .ctors instead of .init_array.
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
