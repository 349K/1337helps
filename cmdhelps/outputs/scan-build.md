# scan-build command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

USAGE: scan-build [options] <build command> [build options]

OPTIONS:

 -analyze-headers

   Also analyze functions in #included files.  By default, such functions
   are skipped unless they are called by functions within the main source file.

 -o <output location>

   Specifies the output directory for analyzer reports. Subdirectories will be
   created as needed to represent separate "runs" of the analyzer. If this
   option is not specified, a directory is created in /tmp (TMPDIR on Mac OS X)
   to store the reports.

 -h
 --help

   Display this message.

 -k
 --keep-going

   Add a "keep on going" option to the specified build command. This option
   currently supports make and xcodebuild. This is a convenience option; one
   can specify this behavior directly using build options.

 --html-title [title]
 --html-title=[title]

   Specify the title used on generated HTML pages. If not specified, a default
   title will be used.

 -plist

   By default the output of scan-build is a set of HTML files. This option
   outputs the results as a set of .plist files.

 -plist-html

   By default the output of scan-build is a set of HTML files. This option
   outputs the results as a set of HTML and .plist files.

 --status-bugs

   By default, the exit status of scan-build is the same as the executed build
   command. Specifying this option causes the exit status of scan-build to be 1
   if it found potential bugs and 0 otherwise.

 --use-cc [compiler path]
 --use-cc=[compiler path]

   scan-build analyzes a project by interposing a "fake compiler", which
   executes a real compiler for compilation and the static analyzer for analysis.
   Because of the current implementation of interposition, scan-build does not
   know what compiler your project normally uses.  Instead, it simply overrides
   the CC environment variable, and guesses your default compiler.

   In the future, this interposition mechanism to be improved, but if you need
   scan-build to use a specific compiler for *compilation* then you can use
   this option to specify a path to that compiler.

 --use-c++ [compiler path]
 --use-c++=[compiler path]

   This is the same as "-use-cc" but for C++ code.

 -v

   Enable verbose output from scan-build. A second and third '-v' increases
   verbosity.

 -V
 --view

   View analysis results in a web browser when the build completes.

ADVANCED OPTIONS:

 -no-failure-reports

   Do not create a 'failures' subdirectory that includes analyzer crash reports
   and preprocessed source files.

 -stats

   Generates visitation statistics for the project being analyzed.

 -maxloop <loop count>

   Specifiy the number of times a block can be visited before giving up.
   Default is 4. Increase for more comprehensive coverage at a cost of speed.

 -internal-stats

   Generate internal analyzer statistics.

 --use-analyzer [Xcode|path to clang]
 --use-analyzer=[Xcode|path to clang]

   scan-build uses the 'clang' executable relative to itself for static
   analysis. One can override this behavior with this option by using the
   'clang' packaged with Xcode (on OS X) or from the PATH.

 --keep-empty

   Don't remove the build results directory even if no issues were reported.

 --override-compiler
   Always resort to the ccc-analyzer even when better interposition methods
   are available.

 -analyzer-config <options>

   Provide options to pass through to the analyzer's -analyzer-config flag.
   Several options are separated with comma: 'key1=val1,key2=val2'

   Available options:
     * stable-report-filename=true or false (default)
       Switch the page naming to:
       report-<filename>-<function/method name>-<id>.html
       instead of report-XXXXXX.html

CONTROLLING CHECKERS:

 A default group of checkers are always run unless explicitly disabled.
 Checkers may be enabled/disabled using the following options:

 -enable-checker [checker name]
 -disable-checker [checker name]

LOADING CHECKERS:

 Loading external checkers using the clang plugin interface:

 -load-plugin [plugin library]

AVAILABLE CHECKERS:

   alpha.core.BoolAssignment       Warn about assigning non-{0,1} values to Boolean variables
   alpha.core.CallAndMessageUnInitRefArg
                                   Check for logical errors for function calls and Objective-C message expressions (e.g., uninitialized arguments, null function pointers, and pointer to undefined variables)
   alpha.core.CastSize             Check when casting a malloc'ed type T, whether the size is a multiple of the size of T
   alpha.core.CastToStruct         Check for cast from non-struct pointer to struct pointer
   alpha.core.FixedAddr            Check for assignment of a fixed address to a pointer
   alpha.core.IdenticalExpr        Warn about unintended use of identical expressions in operators
   alpha.core.PointerArithm        Check for pointer arithmetic on locations other than array elements
   alpha.core.PointerSub           Check for pointer subtractions on two pointers pointing to different memory chunks
   alpha.core.SizeofPtr            Warn about unintended use of sizeof() on pointer expressions
   alpha.core.TestAfterDivZero     Check for division by variable that is later compared against 0. Either the comparison is useless or there is division by zero.
   alpha.cplusplus.VirtualCall     Check virtual function calls during construction or destruction
   alpha.deadcode.UnreachableCode  Check unreachable code
   alpha.osx.cocoa.Dealloc         Warn about Objective-C classes that lack a correct implementation of -dealloc
   alpha.osx.cocoa.DirectIvarAssignment
                                   Check for direct assignments to instance variables
   alpha.osx.cocoa.DirectIvarAssignmentForAnnotatedFunctions
                                   Check for direct assignments to instance variables in the methods annotated with objc_no_direct_instance_variable_assignment
   alpha.osx.cocoa.InstanceVariableInvalidation
                                   Check that the invalidatable instance variables are invalidated in the methods annotated with objc_instance_variable_invalidator
   alpha.osx.cocoa.MissingInvalidationMethod
                                   Check that the invalidation methods are present in classes that contain invalidatable instance variables
   alpha.security.ArrayBound       Warn about buffer overflows (older checker)
   alpha.security.ArrayBoundV2     Warn about buffer overflows (newer checker)
   alpha.security.MallocOverflow   Check for overflows in the arguments to malloc()
   alpha.security.ReturnPtrRange   Check for an out-of-bound pointer being returned to callers
   alpha.security.taint.TaintPropagation
                                   Generate taint information used by other checkers
   alpha.unix.Chroot               Check improper use of chroot
   alpha.unix.MallocWithAnnotations
                                   Check for memory leaks, double free, and use-after-free problems. Traces memory managed by malloc()/free(). Assumes that all user-defined functions which might free a pointer are annotated.
   alpha.unix.PthreadLock          Simple lock -> unlock checker
   alpha.unix.SimpleStream         Check for misuses of stream APIs
   alpha.unix.Stream               Check stream handling functions
   alpha.unix.cstring.BufferOverlap
                                   Checks for overlap in two buffer arguments
   alpha.unix.cstring.NotNullTerminated
                                   Check for arguments which are not null-terminating strings
   alpha.unix.cstring.OutOfBounds  Check for out-of-bounds access in string functions
 + core.CallAndMessage             Check for logical errors for function calls and Objective-C message expressions (e.g., uninitialized arguments, null function pointers)
 + core.DivideZero                 Check for division by zero
 + core.DynamicTypePropagation     Generate dynamic type information
 + core.NonNullParamChecker        Check for null pointers passed as arguments to a function whose arguments are references or marked with the 'nonnull' attribute
 + core.NullDereference            Check for dereferences of null pointers
 + core.StackAddressEscape         Check that addresses to stack memory do not escape the function
 + core.UndefinedBinaryOperatorResult
                                   Check for undefined results of binary operators
 + core.VLASize                    Check for declarations of VLA of undefined or zero size
 + core.builtin.BuiltinFunctions   Evaluate compiler builtin functions (e.g., alloca())
 + core.builtin.NoReturnFunctions  Evaluate "panic" functions that are known to not return to the caller
 + core.uninitialized.ArraySubscript
                                   Check for uninitialized values used as array subscripts
 + core.uninitialized.Assign       Check for assigning uninitialized values
 + core.uninitialized.Branch       Check for uninitialized values used as branch conditions
 + core.uninitialized.CapturedBlockVariable
                                   Check for blocks that capture uninitialized values
 + core.uninitialized.UndefReturn  Check for uninitialized values being returned to the caller
 + cplusplus.NewDelete             Check for double-free and use-after-free problems. Traces memory managed by new/delete.
 + cplusplus.NewDeleteLeaks        Check for memory leaks. Traces memory managed by new/delete.
 + deadcode.DeadStores             Check for values stored to variables that are never read afterwards
   debug.ConfigDumper              Dump config table
   debug.DumpCFG                   Display Control-Flow Graphs
   debug.DumpCallGraph             Display Call Graph
   debug.DumpCalls                 Print calls as they are traversed by the engine
   debug.DumpDominators            Print the dominance tree for a given CFG
   debug.DumpLiveVars              Print results of live variable analysis
   debug.DumpTraversal             Print branch conditions as they are traversed by the engine
   debug.ExprInspection            Check the analyzer's understanding of expressions
   debug.Stats                     Emit warnings with analyzer statistics
   debug.TaintTest                 Mark tainted symbols as such.
   debug.ViewCFG                   View Control-Flow Graphs using GraphViz
   debug.ViewCallGraph             View Call Graph using GraphViz
   debug.ViewExplodedGraph         View Exploded Graphs using GraphViz
   llvm.Conventions                Check code for LLVM codebase conventions
   osx.API                         Check for proper uses of various Apple APIs
   osx.SecKeychainAPI              Check for proper uses of Secure Keychain APIs
   osx.cocoa.AtSync                Check for nil pointers used as mutexes for @synchronized
   osx.cocoa.ClassRelease          Check for sending 'retain', 'release', or 'autorelease' directly to a Class
   osx.cocoa.IncompatibleMethodTypes
                                   Warn about Objective-C method signatures with type incompatibilities
   osx.cocoa.Loops                 Improved modeling of loops using Cocoa collection types
   osx.cocoa.MissingSuperCall      Warn about Objective-C methods that lack a necessary call to super
   osx.cocoa.NSAutoreleasePool     Warn for suboptimal uses of NSAutoreleasePool in Objective-C GC mode
   osx.cocoa.NSError               Check usage of NSError** parameters
   osx.cocoa.NilArg                Check for prohibited nil arguments to ObjC method calls
   osx.cocoa.NonNilReturnValue     Model the APIs that are guaranteed to return a non-nil value
   osx.cocoa.RetainCount           Check for leaks and improper reference count management
   osx.cocoa.SelfInit              Check that 'self' is properly initialized inside an initializer method
   osx.cocoa.UnusedIvars           Warn about private ivars that are never used
   osx.cocoa.VariadicMethodTypes   Check for passing non-Objective-C types to variadic collection initialization methods that expect only Objective-C types
   osx.coreFoundation.CFError      Check usage of CFErrorRef* parameters
   osx.coreFoundation.CFNumber     Check for proper uses of CFNumberCreate
   osx.coreFoundation.CFRetainRelease
                                   Check for null arguments to CFRetain/CFRelease/CFMakeCollectable
   osx.coreFoundation.containers.OutOfBounds
                                   Checks for index out-of-bounds when using 'CFArray' API
   osx.coreFoundation.containers.PointerSizedValues
                                   Warns if 'CFArray', 'CFDictionary', 'CFSet' are created with non-pointer-size values
   security.FloatLoopCounter       Warn on using a floating point value as a loop counter (CERT: FLP30-C, FLP30-CPP)
 + security.insecureAPI.UncheckedReturn
                                   Warn on uses of functions whose return values must be always checked
 + security.insecureAPI.getpw      Warn on uses of the 'getpw' function
 + security.insecureAPI.gets       Warn on uses of the 'gets' function
 + security.insecureAPI.mkstemp    Warn when 'mkstemp' is passed fewer than 6 X's in the format string
 + security.insecureAPI.mktemp     Warn on uses of the 'mktemp' function
   security.insecureAPI.rand       Warn on uses of the 'rand', 'random', and related functions
   security.insecureAPI.strcpy     Warn on uses of the 'strcpy' and 'strcat' functions
 + security.insecureAPI.vfork      Warn on uses of the 'vfork' function
 + unix.API                        Check calls to various UNIX/Posix functions
 + unix.Malloc                     Check for memory leaks, double free, and use-after-free problems. Traces memory managed by malloc()/free().
 + unix.MallocSizeof               Check for dubious malloc arguments involving sizeof
 + unix.MismatchedDeallocator      Check for mismatched deallocators.
 + unix.cstring.BadSizeArg         Check the size argument passed into C string functions for common erroneous patterns
 + unix.cstring.NullArg            Check for null pointers being passed as arguments to C string functions

NOTE: "+" indicates that an analysis is enabled by default.

BUILD OPTIONS

 You can specify any build option acceptable to the build command.

EXAMPLE

 scan-build -o /tmp/myhtmldir make -j4

The above example causes analysis reports to be deposited into a subdirectory
of "/tmp/myhtmldir" and to run "make" with the "-j4" option. A different
subdirectory is created each time scan-build analyzes a project. The analyzer
should support most parallel builds, but not distributed builds.


~~~
