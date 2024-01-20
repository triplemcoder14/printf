# This algorithm essentially parses the format string and processes each conversion specifier accordingly.


The printf() function prints output to stdout, according to format and other arguments passed to printf(). The string format consists of two types of items - characters that will be printed to the screen, and format commands that define how the other arguments to printf() are displayed. You specify a format string with text in it and "special" characters that map to the other arguments of printf().

The prototype of this function is: int _printf(const char format, ...);

This means that it has one mandatory format argument, and an extra number of arguments that can be none, or many.

Format of the format string

The format string is a character string starting and ending with double quotes. The format string comprises zero or more directives; ordinary characters (not %), and conversion specifications, each of which results in fetching zero or more subsequent arguments.

The character % introduces each conversion specification and ends with a conversion specifier. In between there may be (in this order):

* An optional field width

* Zero or more flags

* An optional precision modifier

* An  optional length modifier
