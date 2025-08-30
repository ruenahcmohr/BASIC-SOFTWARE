# BASIC-SOFTWARE
software written in basic for small computers.


cats.bas is my cats game, the target is nascom basic 4.7b running on a 3.636MHz Z80. 
Please feel free to port this to other BASICs and make tweaks.

  V2:  
  - CLS is abstracted
  - RND is abstracted
  - I removed the on x goto, and replaced it with DATA (a bit more portable?)
   


PORTING NOTES:

1) line block 7k is an abstraction for clearing the screen
if you do not have CLS(), the escape sequence may work for serial terminals

2) line block 8k is an abstraction for RND(), as in nascom basic you 
call RND(1) to get 0-0.99 as a float
But in other BASICs you use the argument to determine the max value as an integer.
cal RND(1000) to get 0-999 as an int.


