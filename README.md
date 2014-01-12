php-repl
========

REPL script for PHP  
Forked from https://gist.github.com/oasynnoum/4771380


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
Files for include are sorted with prefix of filename as integer number.
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
alias of ```strlen()```

### h($var)
dump variable value as hex string.







