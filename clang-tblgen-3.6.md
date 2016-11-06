# clang-tblgen-3.6 command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

USAGE: clang-tblgen-3.6 [options] <input file>

OPTIONS:
  -I=<directory>                                       - Directory of include files
  -d=<filename>                                        - Dependency filename
  Action to perform:
    -gen-clang-attr-classes                            - Generate clang attribute clases
    -gen-clang-attr-parser-string-switches             - Generate all parser-related attribute string switches
    -gen-clang-attr-impl                               - Generate clang attribute implementations
    -gen-clang-attr-list                               - Generate a clang attribute list
    -gen-clang-attr-pch-read                           - Generate clang PCH attribute reader
    -gen-clang-attr-pch-write                          - Generate clang PCH attribute writer
    -gen-clang-attr-has-attribute-impl                 - Generate a clang attribute spelling list
    -gen-clang-attr-spelling-index                     - Generate a clang attribute spelling index
    -gen-clang-attr-ast-visitor                        - Generate a recursive AST visitor for clang attributes
    -gen-clang-attr-template-instantiate               - Generate a clang template instantiate code
    -gen-clang-attr-parsed-attr-list                   - Generate a clang parsed attribute list
    -gen-clang-attr-parsed-attr-impl                   - Generate the clang parsed attribute helpers
    -gen-clang-attr-parsed-attr-kinds                  - Generate a clang parsed attribute kinds
    -gen-clang-attr-dump                               - Generate clang attribute dumper
    -gen-clang-diags-defs                              - Generate Clang diagnostics definitions
    -gen-clang-diag-groups                             - Generate Clang diagnostic groups
    -gen-clang-diags-index-name                        - Generate Clang diagnostic name index
    -gen-clang-comment-nodes                           - Generate Clang AST comment nodes
    -gen-clang-decl-nodes                              - Generate Clang AST declaration nodes
    -gen-clang-stmt-nodes                              - Generate Clang AST statement nodes
    -gen-clang-sa-checkers                             - Generate Clang Static Analyzer checkers
    -gen-clang-comment-html-tags                       - Generate efficient matchers for HTML tag names that are used in documentation comments
    -gen-clang-comment-html-tags-properties            - Generate efficient matchers for HTML tag properties
    -gen-clang-comment-html-named-character-references - Generate function to translate named character references to UTF-8 sequences
    -gen-clang-comment-command-info                    - Generate command properties for commands that are used in documentation comments
    -gen-clang-comment-command-list                    - Generate list of commands that are used in documentation comments
    -gen-arm-neon                                      - Generate arm_neon.h for clang
    -gen-arm-neon-sema                                 - Generate ARM NEON sema support for clang
    -gen-arm-neon-test                                 - Generate ARM NEON tests for clang
    -gen-attr-docs                                     - Generate attribute documentation
  -help                                                - Display available options (-help-hidden for more)
  -o=<filename>                                        - Output filename
  -version                                             - Display the version of this program

~~~
