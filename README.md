php-repl
========

REPL(Read–eval–print loop) script for PHP  
Forked from https://gist.github.com/oasynnoum/4771380  
The better way is to use interactive mode if your PHP has supported it.
To get more information about PHP interactive mode see next link.
http://php.net/manual/en/features.commandline.interactive.php

INSTALL
-------

    $ git clone https://github.com/oasynnoum/php-repl.git
    $ chmod +x ./php-repl/repl.php
    $ ln -s ~/bin/php-repl ./php-repl/repl.php
    $ php-repl


SETUP REPL
----------

When before entering loop, the REPL script include files.  
If you type fixed code every time, exclude these code to a PHP file, and save it to php-repl/include directory.  
Files for including are sorted with prefix of filename as integer number.
You may be numbering files as you need.  
For example,

    include/1-setup.php
    include/4-func.php
    include/5-vars.php


FUNCTIONS
---------

### d($var, ...)
alias of ```var_dump()```

### l($var)
print result of ```strlen()```

### h($var)
dump variable value as hex string.


TIPS
----

If line ends with backslash, you can continue to input next line.

    $ php-repl
    > function foo() {\
    >     print __FUNCTION__ . PHP_EOL;\
    > }
    > foo();
    foo
    >


THANKS
------

Code highlighting function has been implemented by [Xeoncross](https://github.com/Xeoncross).




