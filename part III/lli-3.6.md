# lli-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: llvm interpreter & dynamic compiler

USAGE: lli-3.6 [options] <input bitcode> <program arguments>...

OPTIONS:
  -O=<char>                                       - Optimization level. [-O0, -O1, -O2, or -O3] (default = '-O2')
  -aarch64-neon-syntax                            - Choose style of NEON code to emit from AArch64 backend:
    =generic                                      -   Emit generic NEON assembly
    =apple                                        -   Emit Apple-style NEON assembly
  -bounds-checking-single-trap                    - Use one trap block per function
  -code-model                                     - Choose code model
    =default                                      -   Target default JIT code model
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
  -disable-lazy-compilation                       - Disable JIT lazy compilation
  -disable-spill-fusing                           - Disable fusing of spill code into instructions
  -enable-cache-manager                           - Use cache manager to save/load mdoules
  -enable-load-pre                                - 
  -enable-misched                                 - Enable the machine instruction scheduling pass.
  -enable-objc-arc-opts                           - enable/disable all ARC Optimizations
  -enable-scoped-noalias                          - 
  -enable-tbaa                                    - 
  -entry-function=<function>                      - Specify the entry function (default = 'main') of the executable
  -exhaustive-register-search                     - Exhaustive Search for registers bypassing the depth and interference cutoffs of last chance recoloring
  -extra-archive=<input archive>                  - Extra archive files to be loaded
  -extra-module=<input bitcode>                   - Extra modules to be loaded
  -extra-object=<input object>                    - Extra object files to be loaded
  -fake-argv0=<executable>                        - Override the 'argv[0]' value passed into the executing program
  -float-abi                                      - Choose float ABI type
    =default                                      -   Target default float ABI type
    =soft                                         -   Soft float ABI (implied by -soft-float)
    =hard                                         -   Hard float ABI (uses FP registers)
  -force-interpreter                              - Force interpretation: disable JIT
  -help                                           - Display available options (-help-hidden for more)
  -internalize-public-api-file=<filename>         - A file containing list of symbol names to preserve
  -internalize-public-api-list=<list>             - A list of symbol names to preserve
  -jit-emit-debug                                 - Emit debug information to debugger
  -join-liveintervals                             - Coalesce copies (default=true)
  -limit-float-precision=<uint>                   - Generate low-precision inline sequences for some float libcalls
  -load=<pluginfilename>                          - Load the specified plugin
  -march=<string>                                 - Architecture to generate assembly for (see --version)
  -mattr=<a1,+a2,-a3,...>                         - Target specific attributes (-mattr=help for details)
  -mc-x86-disable-arith-relaxation                - Disable relaxation of arithmetic instruction for X86
  -mcjit-remote-process=<filename>                - Specify the filename of the process to launch for remote MCJIT execution.  If none is specified,
                                                    	remote execution will be simulated in-process.
  -mcpu=<cpu-name>                                - Target a specific cpu type (-mcpu=help for details)
  -mips16-constant-islands                        - MIPS: mips16 constant islands enable.
  -mips16-hard-float                              - MIPS: mips16 hard float enable.
  -mno-ldc1-sdc1                                  - Expand double precision loads and stores to their single precision counterparts
  -mtriple=<string>                               - Override target triple for module
  -no-discriminators                              - Disable generation of discriminator information.
  -nvptx-sched4reg                                - NVPTX Specific: schedule for register pressue
  -object-cache-dir=<string>                      - Directory to store cached object files (must be user writable)
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
  -remote-mcjit                                   - Execute MCJIT'ed code in a separate process.
  -rewrite-map-file=<filename>                    - Symbol Rewrite Map
  -rng-seed=<seed>                                - Seed for the random number generator
  -sample-profile-max-propagate-iterations=<uint> - Maximum number of iterations to go through when propagating sample block/edge weights through the CFG.
  -soft-float                                     - Generate software floating point library calls
  -stackmap-version=<int>                         - Specify the stackmap encoding version (default = 1)
  -stats                                          - Enable statistics output from program (available with Asserts)
  -time-passes                                    - Time each pass, printing elapsed time for each on exit
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
