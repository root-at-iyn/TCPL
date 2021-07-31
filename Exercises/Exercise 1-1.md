Exercise 1-1 requries the student to compile a simple hello world c program, but leave require syntax out in the process. The lesson here is for the student to see what compliation errors look like, and to affirm the lessons point on required syntax. 

For example, the following hello.c progam was complied, but without a semicolon to end the print statement. In C, a semicolon is required to terminate the statement. This is shown below:


```
/* Excercise 1-1. Run the "hello, world" program on your system. Experiment with leaving out parts of the program, to see what error messages you get. */


// hello.c

#include <stdio.h>

main ()
{
        printf("hello")


}

```

When compiling this program,  the GCC complier will produce the following error:

![[hello_no_semicolcon_complie_error.png]]
![Compilation Error](/Images/hello_no_semicolcon_complie_error.png?raw=true "Compliation Error")
