# bugpoint-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: LLVM automatic testcase reducer. See
http://llvm.org/cmds/bugpoint.html for more information.

USAGE: bugpoint-3.6 [options] --args <program arguments>... --tool-args <tool arguments>... --safe-tool-args <safe-tool arguments>... --gcc-tool-args <gcc-tool arguments>... --opt-args <opt arguments>... <input llvm ll/bc files>

OPTIONS:
  -O1                                             - Optimization level 1. Identical to 'opt -O1'
  -O2                                             - Optimization level 2. Identical to 'opt -O2'
  -O3                                             - Optimization level 3. Identical to 'opt -O3'
  -Xlinker=<string>                               - Additional arguments to pass to the linker
  -aarch64-neon-syntax                            - Choose style of NEON code to emit from AArch64 backend:
    =generic                                      -   Emit generic NEON assembly
    =apple                                        -   Emit Apple-style NEON assembly
  -abs-tolerance=<number>                         - Absolute error tolerated
  -additional-so=<string>                         - Additional shared objects to load into executing programs
  -append-exit-code                               - Append the exit code to the output so it gets diff'd too
  -args=<string>                                  - <program arguments>...
  -bounds-checking-single-trap                    - Use one trap block per function
  -color                                          - use colored syntax highlighting (default=autodetect)
  -compile-command=<string>                       - Command to compile the bitcode (use with -compile-custom) (default: llc)
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
  -disable-block-extraction                       - Don't extract blocks when searching for miscompilations
  -disable-dce                                    - Do not use the -dce pass to reduce testcases
  -disable-global-remove                          - Do not remove global variables
  -disable-loop-extraction                        - Don't extract loops when searching for miscompilations
  -disable-simplifycfg                            - Do not use the -simplifycfg pass to reduce testcases
  -disable-spill-fusing                           - Disable fusing of spill code into instructions
  -enable-load-pre                                - 
  -enable-misched                                 - Enable the machine instruction scheduling pass.
  -enable-objc-arc-opts                           - enable/disable all ARC Optimizations
  -enable-scoped-noalias                          - 
  -enable-tbaa                                    - 
  -enable-valgrind                                - Run optimizations through valgrind
  -exec-command=<string>                          - Command to execute the bitcode (use with -run-custom) (default: simulate)
  -exhaustive-register-search                     - Exhaustive Search for registers bypassing the depth and interference cutoffs of last chance recoloring
  -find-bugs                                      - Run many different optimization sequences on program to find bugs
  -gcc=<string>                                   - The gcc binary to use. (default 'gcc')
  -gcc-tool-args=<string>                         - <gcc-tool arguments>...
  -help                                           - Display available options (-help-hidden for more)
  -input=<string>                                 - Filename to pipe in as stdin (default: /dev/null)
  -internalize-public-api-file=<filename>         - A file containing list of symbol names to preserve
  -internalize-public-api-list=<list>             - A list of symbol names to preserve
  -join-liveintervals                             - Coalesce copies (default=true)
  -keep-main                                      - Force function reduction to keep main
  -limit-float-precision=<uint>                   - Generate low-precision inline sequences for some float libcalls
  -load=<pluginfilename>                          - Load the specified plugin
  Passes available:
    -aa-eval                                      - Exhaustive Alias Analysis Precision Evaluator
    -adce                                         - Aggressive Dead Code Elimination
    -add-discriminators                           - Add DWARF path discriminators
    -alignment-from-assumptions                   - Alignment from assumptions
    -alloca-hoisting                              - Hoisting alloca instructions in non-entry blocks to the entry block
    -always-inline                                - Inliner for always_inline functions
    -argpromotion                                 - Promote 'by reference' arguments to scalars
    -asan                                         - AddressSanitizer: detects use-after-free and out-of-bounds bugs.
    -asan-module                                  - AddressSanitizer: detects use-after-free and out-of-bounds bugs.ModulePass
    -assumption-cache-tracker                     - Assumption Cache Tracker
    -barrier                                      - A No-Op Barrier Pass
    -basicaa                                      - Basic Alias Analysis (stateless AA impl)
    -basiccg                                      - CallGraph Construction
    -bb-vectorize                                 - Basic-Block Vectorization
    -block-freq                                   - Block Frequency Analysis
    -bounds-checking                              - Run-time bounds checking
    -branch-prob                                  - Branch Probability Analysis
    -break-crit-edges                             - Break critical edges in CFG
    -cfl-aa                                       - CFL-Based AA implementation
    -consthoist                                   - Constant Hoisting
    -constmerge                                   - Merge Duplicate Global Constants
    -constprop                                    - Simple constant propagation
    -correlated-propagation                       - Value Propagation
    -cost-model                                   - Cost Model Analysis
    -count-aa                                     - Count Alias Analysis Query Responses
    -da                                           - Dependence Analysis
    -datalayout                                   - Data Layout
    -dce                                          - Dead Code Elimination
    -deadargelim                                  - Dead Argument Elimination
    -deadarghaX0r                                 - Dead Argument Hacking (BUGPOINT USE ONLY; DO NOT USE)
    -debug-aa                                     - AA use debugger
    -delinearize                                  - Delinearization
    -dfsan                                        - DataFlowSanitizer: dynamic data flow analysis.
    -die                                          - Dead Instruction Elimination
    -domfrontier                                  - Dominance Frontier Construction
    -domtree                                      - Dominator Tree Construction
    -dot-callgraph                                - Print call graph to 'dot' file
    -dot-cfg                                      - Print CFG of function to 'dot' file
    -dot-cfg-only                                 - Print CFG of function to 'dot' file (with no function bodies)
    -dot-dom                                      - Print dominance tree of function to 'dot' file
    -dot-dom-only                                 - Print dominance tree of function to 'dot' file (with no function bodies)
    -dot-postdom                                  - Print postdominance tree of function to 'dot' file
    -dot-postdom-only                             - Print postdominance tree of function to 'dot' file (with no function bodies)
    -dot-regions                                  - Print regions of function to 'dot' file
    -dot-regions-only                             - Print regions of function to 'dot' file (with no function bodies)
    -dse                                          - Dead Store Elimination
    -early-cse                                    - Early CSE
    -extract-blocks                               - Extract Basic Blocks From Module (for bugpoint use)
    -flattencfg                                   - Flatten the CFG
    -function_tti                                 - Function TargetTransformInfo
    -functionattrs                                - Deduce function attributes
    -globaldce                                    - Dead Global Elimination
    -globalopt                                    - Global Variable Optimizer
    -globalsmodref-aa                             - Simple mod/ref analysis for globals
    -gvn                                          - Global Value Numbering
    -indvars                                      - Induction Variable Simplification
    -inline                                       - Function Integration/Inlining
    -inline-cost                                  - Inline Cost Analysis
    -insert-gcov-profiling                        - Insert instrumentation for GCOV profiling
    -instcombine                                  - Combine redundant instructions
    -instcount                                    - Counts the various types of Instructions
    -instnamer                                    - Assign names to anonymous instructions
    -instrprof                                    - Frontend instrumentation-based coverage lowering.
    -instsimplify                                 - Remove redundant instructions
    -internalize                                  - Internalize Global Symbols
    -intervals                                    - Interval Partition Construction
    -ipconstprop                                  - Interprocedural constant propagation
    -ipsccp                                       - Interprocedural Sparse Conditional Constant Propagation
    -iv-users                                     - Induction Variable Users
    -jump-instr-table-info                        - Jump-Instruction Table Info
    -jump-threading                               - Jump Threading
    -lazy-value-info                              - Lazy Value Information Analysis
    -lcssa                                        - Loop-Closed SSA Form Pass
    -libcall-aa                                   - LibCall Alias Analysis
    -licm                                         - Loop Invariant Code Motion
    -lint                                         - Statically lint-checks LLVM IR
    -load-combine                                 - Combine Adjacent Loads
    -loop-deletion                                - Delete dead loops
    -loop-extract                                 - Extract loops into new functions
    -loop-extract-single                          - Extract at most one loop into a new function
    -loop-idiom                                   - Recognize loop idioms
    -loop-instsimplify                            - Simplify instructions in loops
    -loop-reduce                                  - Loop Strength Reduction
    -loop-reroll                                  - Reroll loops
    -loop-rotate                                  - Rotate Loops
    -loop-simplify                                - Canonicalize natural loops
    -loop-unroll                                  - Unroll loops
    -loop-unswitch                                - Unswitch loops
    -loop-vectorize                               - Loop Vectorization
    -loops                                        - Natural Loop Information
    -lower-expect                                 - Lower 'expect' Intrinsics
    -loweratomic                                  - Lower atomic intrinsics to non-atomic form
    -lowerinvoke                                  - Lower invoke and unwind, for unwindless code generators
    -lowerswitch                                  - Lower SwitchInst's to branches
    -mem2reg                                      - Promote Memory to Register
    -memcpyopt                                    - MemCpy Optimization
    -memdep                                       - Memory Dependence Analysis
    -mergefunc                                    - Merge Functions
    -mergereturn                                  - Unify function exit nodes
    -metarenamer                                  - Assign new names to everything
    -mldst-motion                                 - MergedLoadStoreMotion
    -module-debuginfo                             - Decodes module-level debug info
    -msan                                         - MemorySanitizer: detects uninitialized reads.
    -no-aa                                        - No Alias Analysis (always returns 'may' alias)
    -notti                                        - No target information
    -objc-arc                                     - ObjC ARC optimization
    -objc-arc-aa                                  - ObjC-ARC-Based Alias Analysis
    -objc-arc-apelim                              - ObjC ARC autorelease pool elimination
    -objc-arc-contract                            - ObjC ARC contraction
    -objc-arc-expand                              - ObjC ARC expansion
    -pa-eval                                      - Evaluate ProvenanceAnalysis on all pairs
    -partial-inliner                              - Partial Inliner
    -partially-inline-libcalls                    - Partially inline calls to library functions
    -postdomtree                                  - Post-Dominator Tree Construction
    -print-alias-sets                             - Alias Set Printer
    -print-bb                                     - Print BB to stderr
    -print-function                               - Print function to stderr
    -print-memdeps                                - Print MemDeps of function
    -print-module                                 - Print module to stderr
    -prune-eh                                     - Remove unused exception handling info
    -reassociate                                  - Reassociate expressions
    -reg2mem                                      - Demote all values to stack slots
    -regions                                      - Detect single entry single exit regions
    -sample-profile                               - Sample Profile loader
    -sancov                                       - SanitizerCoverage: TODO.ModulePass
    -scalar-evolution                             - Scalar Evolution Analysis
    -scalarizer                                   - Scalarize vector operations
    -scalarrepl                                   - Scalar Replacement of Aggregates (DT)
    -scalarrepl-ssa                               - Scalar Replacement of Aggregates (SSAUp)
    -sccp                                         - Sparse Conditional Constant Propagation
    -scev-aa                                      - ScalarEvolution-based Alias Analysis
    -scoped-noalias                               - Scoped NoAlias Alias Analysis
    -separate-const-offset-from-gep               - Split GEPs to a variadic base and a constant offset for better CSE
    -simplifycfg                                  - Simplify the CFG
    -sink                                         - Code sinking
    -slp-vectorizer                               - SLP Vectorizer
    -sroa                                         - Scalar Replacement Of Aggregates
    -strip                                        - Strip all symbols from a module
    -strip-dead-debug-info                        - Strip debug info for unused symbols
    -strip-dead-prototypes                        - Strip Unused Function Prototypes
    -strip-debug-declare                          - Strip all llvm.dbg.declare intrinsics
    -strip-nondebug                               - Strip all symbols, except dbg symbols, from a module
    -structurizecfg                               - Structurize the CFG
    -tailcallelim                                 - Tail Call Elimination
    -targetlibinfo                                - Target Library Information
    -tbaa                                         - Type-Based Alias Analysis
    -tsan                                         - ThreadSanitizer: detects data races.
    -verify                                       - Module Verifier
    -view-callgraph                               - View call graph
    -view-cfg                                     - View CFG of function
    -view-cfg-only                                - View CFG of function (with no function bodies)
    -view-dom                                     - View dominance tree of function
    -view-dom-only                                - View dominance tree of function (with no function bodies)
    -view-postdom                                 - View postdominance tree of function
    -view-postdom-only                            - View postdominance tree of function (with no function bodies)
    -view-regions                                 - View regions of function
    -view-regions-only                            - View regions of function (with no function bodies)
  -mc-x86-disable-arith-relaxation                - Disable relaxation of arithmetic instruction for X86
  -mips16-constant-islands                        - MIPS: mips16 constant islands enable.
  -mips16-hard-float                              - MIPS: mips16 hard float enable.
  -mlimit=<MBytes>                                - Maximum amount of memory to use. 0 disables check. Defaults to 300MB (800MB under valgrind).
  -mno-ldc1-sdc1                                  - Expand double precision loads and stores to their single precision counterparts
  -mtriple=<string>                               - Override target triple for module
  -no-discriminators                              - Disable generation of discriminator information.
  -nvptx-sched4reg                                - NVPTX Specific: schedule for register pressue
  -opt-args=<string>                              - <opt arguments>...
  -opt-command=<string>                           - Path to opt. (default: search path for 'opt'.)
  -output=<string>                                - Specify a reference program output (for miscompilation detection)
  -output-prefix=<string>                         - Prefix to use for outputs (default: 'bugpoint')
  -print-after-all                                - Print IR after each pass
  -print-before-all                               - Print IR before each pass
  -print-machineinstrs=<pass-name>                - Print machine instrs
  -regalloc                                       - Register allocator to use
    =default                                      -   pick register allocator based on -O option
    =basic                                        -   basic register allocator
    =fast                                         -   fast register allocator
    =greedy                                       -   greedy register allocator
    =pbqp                                         -   PBQP register allocator
  -rel-tolerance=<number>                         - Relative error tolerated
  -remote-client=<string>                         - Remote execution client (rsh/ssh)
  -remote-extra-options=<string>                  - Remote execution (rsh/ssh) extra options
  -remote-host=<string>                           - Remote execution (rsh/ssh) host
  -remote-port=<string>                           - Remote execution (rsh/ssh) port
  -remote-user=<string>                           - Remote execution (rsh/ssh) user id
  -rewrite-map-file=<filename>                    - Symbol Rewrite Map
  -rng-seed=<seed>                                - Seed for the random number generator
  Specify the "test" i.e. suspect back-end:
    -auto                                         - Use best guess
    -run-int                                      - Execute with the interpreter
    -run-jit                                      - Execute with JIT
    -run-llc                                      - Compile with LLC
    -run-llc-ia                                   - Compile with LLC with integrated assembler
    -llc-safe                                     - Use LLC for all
    -compile-custom                               - Use -compile-command to define a command to compile the bitcode. Useful to avoid linking.
    -run-custom                                   - Use -exec-command to define a command to execute the bitcode. Useful for cross-compilation.
  Specify "safe" i.e. known-good backend:
    -safe-auto                                    - Use best guess
    -safe-run-llc                                 - Compile with LLC
    -safe-run-custom                              - Use -exec-command to define a command to execute the bitcode. Useful for cross-compilation.
  -safe-path=<string>                             - Specify the path to the "safe" backend program
  -safe-tool-args=<string>                        - <safe-tool arguments>...
  -sample-profile-max-propagate-iterations=<uint> - Maximum number of iterations to go through when propagating sample block/edge weights through the CFG.
  -save-temps                                     - Save temporary files
  -silence-passes                                 - Suppress output of running passes (both stdout and stderr)
  -stackmap-version=<int>                         - Specify the stackmap encoding version (default = 1)
  -stats                                          - Enable statistics output from program (available with Asserts)
  -std-link-opts                                  - Include the standard link time optimizations
  -time-passes                                    - Time each pass, printing elapsed time for each on exit
  -timeout=<seconds>                              - Number of seconds program is allowed to run before it is killed (default is 300s), 0 disables timeout
  -tool-args=<string>                             - <tool arguments>...
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
