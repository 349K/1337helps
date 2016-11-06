# clang-check command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

USAGE: clang-check [options] <source0> [... <sourceN>]

OPTIONS:

General options:

  -help                      - Display available options (-help-hidden for more)
  -help-list                 - Display list of available options (-help-list-hidden for more)
  -version                   - Display the version of this program

clang-check options:

  -analyze                   - Run static analysis engine
  -ast-dump                  - Build ASTs and then debug dump them
  -ast-dump-filter=<string>  - Use with -ast-dump or -ast-print to dump/print only AST declaration nodes having a certain substring in a qualified name. Use -ast-list to list all filterable declaration node names.
  -ast-list                  - Build ASTs and print the list of declaration node qualified names
  -ast-print                 - Build ASTs and then pretty-print them
  -extra-arg=<string>        - Additional argument to append to the compiler command line
  -extra-arg-before=<string> - Additional argument to prepend to the compiler command line
  -fix-what-you-can          - Apply fix-it advice even in the presence of unfixable errors
  -fixit                     - Apply fix-it advice to the input source
  -p=<string>                - Build path

-p <build-path> is used to read a compile command database.

	For example, it can be a CMake build directory in which a file named
	compile_commands.json exists (use -DCMAKE_EXPORT_COMPILE_COMMANDS=ON
	CMake option to get this output). When no build path is specified,
	a search for compile_commands.json will be attempted through all
	parent paths of the first input file . See:
	http://clang.llvm.org/docs/HowToSetupToolingForLLVM.html for an
	example of setting up Clang Tooling on a source tree.

<source0> ... specify the paths of source files. These paths are
	looked up in the compile command database. If the path of a file is
	absolute, it needs to point into CMake's source tree. If the path is
	relative, the current working directory needs to be in the CMake
	source tree and the file must be in a subdirectory of the current
	working directory. "./" prefixes in the relative files will be
	automatically removed, but the rest of a relative path must be a
	suffix of a path in the compile command database.

	For example, to run clang-check on all files in a subtree of the
	source tree, use:

	  find path/in/subtree -name '*.cpp'|xargs clang-check

	or using a specific build path:

	  find path/in/subtree -name '*.cpp'|xargs clang-check -p build/path

	Note, that path/in/subtree and current directory should follow the
	rules described above.


~~~
