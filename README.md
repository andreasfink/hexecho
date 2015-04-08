
##hexecho##

hereto is a tool to display characters based on their hexadecimal values. For example you see the character sequence 414243 somewhere being displayed in hex and you want to quickly know what this represents then you can copy and paste this to the command line prefixed with hexecho to display it.

Example:

*hexecho 414243* 

 outputs

 *ABC*

same is true for 
*hexecho 41 42 43*
 *hexecho Z414243Z*

any characters not in the range 0-9 or A-F/a-f are ignored (except the option -r ).
 

*hexecho 010203*

outputs

*\x01\x02\x03*


if you pass -r it will output the hex bytes directly and will not escape non printable characters. That's a quick way to write arbitrary hexadecimal data into a file

   *hexecho -r 010203 > mydata*

now the file mydata contains the bytes 01 02 03
