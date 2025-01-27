# pcap-notes
Notes for my PCAP certification exam.

## to-do
* go through training video, take notes
* take practice test
* identify weak points
* make flash cards
* study
* take practice test again
* take PCAP exam

## primary source
https://www.udemy.com/course/python-pcap/

## PCAP sections
* modules and packages
* strings
* OOP
* exceptions
* misc

## modules and packages
* intro to modules
    * decomposition (breaking it down into chunks/separate files)
    * need to tie it all together
    * module contains definitions and statements that are used by a larger program (like setup.py, for example, in client apps)
    * [Python Standard Library](https://docs.python.org/3/library/index.html)
* importing
    * ```import sys``` for example
    * should be at top of the file
    * can use multiple ```import``` or sep module names with commas
    * can import just parts of a module
        * ```from``` module ```import``` functionality
    * your locally defined functions override imported functions. ie.: if you have ```from sys import exit``` and have defined another function called ```exit()```, calling that function will trigger your locally defined function first
    * you can use splat to import everything from a module (```from sys import *```), but it's dangerous because some modules will be replaced
    * ```import sys``` means you have to call functions like ```sys.exit()``` rather than ```exit()```
    * ```import sys as s``` is aliasing -- you can change the prefix you us, (like df for ```DataFrames```)
    * ```from sys import exit as bye_bye``` replaces exit() with bye_bye(), but it's a shitty idea to do this because it becomes very nonstandard
* math module
    * only need to know 6 functions for PCAP
    * rounding functions
        * ```ceil()``` -- rounds up to nearest integer, never less than original number
        * ```floor()``` -- always rounds down to nearest number, never greater than original number
        * ```trunc()``` -- just chops the decimal part and returns integer form
    * ```factorial()``` 3! = 3 * 2 * 1
    * ```sqrt()``` square root -- always returns float
    * ```hypot(x, y)``` find longest side of a right triangle, if you know length of short sides
* random module

* further stuff on random.sample
* platform module
* creating your own
* module locations
* using packages
