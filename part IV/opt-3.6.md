# opt-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

OVERVIEW: llvm .bc -> .bc modular optimizer and analysis printer

USAGE: opt-3.6 [options] <input bitcode file>

OPTIONS:
  -O1                                             - Optimization level 1. Similar to clang -O1
  -O2                                             - Optimization level 2. Similar to clang -O2
  -O3                                             - Optimization level 3. Similar to clang -O3
  -Os                                             - Like -O2 with extra optimizations for size. Similar to clang -Os
  -Oz                                             - Like -Os but reduces code size further. Similar to clang -Oz
  -S                                              - Write output as LLVM assembly
  -aarch64-neon-syntax                            - Choose style of NEON code to emit from AArch64 backend:
    =generic                                      -   Emit generic NEON assembly
    =apple                                        -   Emit Apple-style NEON assembly
  -analyze                                        - Only perform analysis, no optimization
  -asm-instrumentation                            - Instrumentation of inline assembly and assembly source files
    =none                                         -   no instrumentation at all
    =address                                      -   instrument instructions with memory arguments
  -asm-show-inst                                  - Emit internal instruction representation to assembly file
  Optimizations available:
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
    -atomic-expand                                - Expand Atomic calls in terms of either load-linked & store-conditional or cmpxchg
    -barrier                                      - A No-Op Barrier Pass
    -basicaa                                      - Basic Alias Analysis (stateless AA impl)
    -basiccg                                      - CallGraph Construction
    -bb-vectorize                                 - Basic-Block Vectorization
    -block-freq                                   - Block Frequency Analysis
    -bounds-checking                              - Run-time bounds checking
    -branch-prob                                  - Branch Probability Analysis
    -break-crit-edges                             - Break critical edges in CFG
    -cfl-aa                                       - CFL-Based AA implementation
    -codegenprepare                               - Optimize for code generation
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
    -generic-to-nvvm                              - Ensure that the global variables are in the global address space
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
    -nvptx-assign-valid-global-names              - Assign valid PTX names to globals
    -nvptx-favor-non-generic                      - Remove unnecessary non-generic-to-generic addrspacecasts
    -nvptx-lower-struct-args                      - Lower structure arguments (NVPTX)
    -nvvm-reflect                                 - Replace occurrences of __nvvm_reflect() calls with 0/1
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
    -print-callgraph                              - Print a call graph
    -print-callgraph-sccs                         - Print SCCs of the Call Graph
    -print-cfg-sccs                               - Print SCCs of each function CFG
    -print-dom-info                               - Dominator Info Printer
    -print-externalfnconstants                    - Print external fn callsites passed constants
    -print-function                               - Print function to stderr
    -print-memdeps                                - Print MemDeps of function
    -print-module                                 - Print module to stderr
    -prune-eh                                     - Remove unused exception handling info
    -reassociate                                  - Reassociate expressions
    -reg2mem                                      - Demote all values to stack slots
    -regions                                      - Detect single entry single exit regions
    -rewrite-symbols                              - Rewrite Symbols
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
  -default-data-layout=<layout-string>            - data layout string to use if not specified by module
  -disable-fp-elim                                - Disable frame pointer elimination optimization
  -disable-inlining                               - Do not run the inliner pass
  -disable-loop-unrolling                         - Disable loop unrolling in all relevant passes
  -disable-loop-vectorization                     - Disable the loop vectorization pass
  -disable-opt                                    - Do not run any optimization passes
  -disable-simplify-libcalls                      - Disable simplify-libcalls
  -disable-slp-vectorization                      - Disable the slp vectorization pass
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
  -f                                              - Enable binary output on terminals
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
  -funit-at-a-time                                - Enable IPO. This corresponds to gcc's -funit-at-a-time
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
  -o=<filename>                                   - Override output filename
  -p                                              - Print module after each transformation
  -print-after-all                                - Print IR after each pass
  -print-before-all                               - Print IR before each pass
  -print-breakpoints-for-testing                  - Print select breakpoints location for testing
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
  -std-link-opts                                  - Include the standard link time optimizations
  -stop-after=<pass-name>                         - Stop compilation after a specific pass
  -strip-debug                                    - Strip debugger symbol info from translation unit
  -tailcallopt                                    - Turn fastcc calls into tail calls by (potentially) changing ABI.
  -thread-model                                   - Choose threading model
    =posix                                        -   POSIX thread model
    =single                                       -   Single thread model
  -time-passes                                    - Time each pass, printing elapsed time for each on exit
  -use-ctors                                      - Use .ctors instead of .init_array.
  -verify-debug-info                              - 
  -verify-dom-info                                - Verify dominator info (time consuming)
  -verify-each                                    - Verify after each transform
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
