# llvm-tblgen-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

USAGE: llvm-tblgen-3.6 [options] <input file>

OPTIONS:
  -I=<directory>         - Directory of include files
  -asmparsernum=<uint>   - Make -gen-asm-parser emit assembly parser #N
  -asmwriternum=<uint>   - Make -gen-asm-writer emit assembly writer #N
  -class=<class name>    - Print Enum list for this class
  -d=<filename>          - Dependency filename
  -help                  - Display available options (-help-hidden for more)
  -match-prefix=<string> - Only match instructions with the given prefix
  -o=<filename>          - Output filename
  -omit-comments         - Do not generate comments
  Action to perform:
    -print-records       - Print all records to stdout (default)
    -gen-emitter         - Generate machine code emitter
    -gen-register-info   - Generate registers and register classes info
    -gen-instr-info      - Generate instruction descriptions
    -gen-callingconv     - Generate calling convention descriptions
    -gen-asm-writer      - Generate assembly writer
    -gen-disassembler    - Generate disassembler
    -gen-pseudo-lowering - Generate pseudo instruction lowering
    -gen-asm-matcher     - Generate assembly instruction matcher
    -gen-dag-isel        - Generate a DAG instruction selector
    -gen-dfa-packetizer  - Generate DFA Packetizer for VLIW targets
    -gen-fast-isel       - Generate a "fast" instruction selector
    -gen-subtarget       - Generate subtarget enumerations
    -gen-intrinsic       - Generate intrinsic information
    -gen-tgt-intrinsic   - Generate target intrinsic information
    -print-enums         - Print enum values for a class
    -print-sets          - Print expanded sets for testing DAG exprs
    -gen-opt-parser-defs - Generate option definitions
    -gen-ctags           - Generate ctags-compatible index
  -version               - Display the version of this program

~~~
