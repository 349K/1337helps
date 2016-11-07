# img2py command Help
 
 This command seen on Linux kali 4.6.0-kali1-amd64 #1 SMP Debian 4.6.4-1kali1 (2016-07-21) x86_64 GNU/Linux. For further information please check [docs.kali.org](docs.kali.org) and have a nice day buddy ;) 

~~~


img2py.py  --  Convert an image to PNG format and embed it in a Python
               module with appropriate code so it can be loaded into
               a program at runtime.  The benefit is that since it is
               Python source code it can be delivered as a .pyc or
               'compiled' into the program using freeze, py2exe, etc.

Usage:

    img2py.py [options] image_file python_file

Options:

    -m <#rrggbb>   If the original image has a mask or transparency defined
                   it will be used by default.  You can use this option to
                   override the default or provide a new mask by specifying
                   a colour in the image to mark as transparent.

    -n <name>      Normally generic names (getBitmap, etc.) are used for the
                   image access functions.  If you use this option you can
                   specify a name that should be used to customize the access
                   fucntions, (getNameBitmap, etc.)

    -c             Maintain a catalog of names that can be used to reference
                   images.  Catalog can be accessed via catalog and 
                   index attributes of the module.  
                   If the -n <name> option is specified then <name>
                   is used for the catalog key and index value, otherwise
                   the filename without any path or extension is used 
                   as the key.

    -a             This flag specifies that the python_file should be appended
                   to instead of overwritten.  This in combination with -n will
                   allow you to put multiple images in one Python source file.

    -i             Also output a function to return the image as a wxIcon.

    -f             Generate code compatible with the old function interface.
                   (This option is ON by default in 2.8, use -F to turn off.)
    
You can also import this module from your Python scripts, and use its img2py()
function. See its docstring for more info.


~~~
