# erubis command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~

erubis - embedded program converter for multi-language
Usage: erubis [..options..] [file ...]
  -h, --help    : help
  -v            : version
  -x            : show converted code
  -X            : show converted code, only ruby code and no text part
  -N            : numbering: add line numbers            (for '-x/-X')
  -U            : unique: compress empty lines to a line (for '-x/-X')
  -C            : compact: remove empty lines            (for '-x/-X')
  -b            : body only: no preamble nor postamble   (for '-x/-X')
  -z            : syntax checking
  -e            : escape (equal to '--E Escape')
  -p pattern    : embedded pattern (default '<% %>')
  -l lang       : convert but no execute (ruby/php/c/cpp/java/scheme/perl/js)
  -E e1,e2,...  : enhancer names (Escape, PercentLine, BiPattern, ...)
  -I path       : library include path
  -K kanji      : kanji code (euc/sjis/utf8) (default none)
  -c context    : context data string (yaml inline style or ruby code)
  -f datafile   : context data file ('*.yaml', '*.yml', or '*.rb')
  -T            : don't expand tab characters in YAML file
  -S            : convert mapping key from string to symbol in YAML file
  -B            : invoke 'result(binding)' instead of 'evaluate(context)'
  --pi=name     : parse '<?name ... ?>' instead of '<% ... %>'
supported properties:
  * (common)
     --escapefunc=nil          : escape function name
     --pattern="<% %>"         : embed pattern
     --trim=true               : trim spaces around <% ... %>
     --preamble=nil            : preamble (no preamble when false)
     --postamble=nil           : postamble (no postamble when false)
     --escape=nil              : escape expression or not in default
  * (basic)
  * (pi)
     --pi="rb"                 : PI (Processing Instrunctions) name
     --embchar="@"             : char for embedded expression pattern('@{...}@')
  * ruby
  * php
  * c
     --indent=""               : indent spaces (ex. '  ')
     --out="stdout"            : output file pointer name
  * cpp
     --indent=""               : indent spaces (ex. '  ')
     --bufvar="_buf"           : buffer variable name
  * java
     --indent=""               : indent spaces (ex. '  ')
     --bufvar="_buf"           : output buffer variable name
     --bufclass="StringBuffer" : output buffer class (ex. 'StringBuilder')
  * scheme
     --func="_add"             : function name (ex. 'display')
  * perl
     --func="print"            : function name
  * javascript
     --docwrite=true           : use 'document.write()' when true

enhancers:
  Array         : return array instead of string
  ArrayBuffer   : use an Array object for buffering (included in Eruby class)
  BiPattern     : another embedded expression pattern (default '[= =]').
  DeleteIndent  : delete indentation of HTML.
  Erbout        : set '_erbout = _buf = "";' to be compatible with ERB.
  Escape        : switch '<%= %>' to escaped and '<%== %>' to unescaped
  HeaderFooter  : allow header/footer in document (ex. '<!--#header: #-->')
  Interpolation : convert '<p><%=text%></p>' into '_buf << %Q`<p>#{text}</p>`'
  NoCode        : remove code and leave text (useful when validating HTML)
  NoText        : remove text and leave code (useful when debugging)
  PercentLine   : regard lines starting with '%' as program code
  PrefixedLine  : regard lines matched to '^[ 	]*%' as program code
  PrintEnabled  : enable to use print function in '<% %>'
  PrintOut      : use print statement instead of '_buf << ...'
  Simplify      : get convert faster but leave spaces around '<% %>'
  Stdout        : use $stdout instead of array buffer or string buffer
  StringBuffer  : use a String object for buffering
  StringIO      : use a StringIO object for buffering

~~~
