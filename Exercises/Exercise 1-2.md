This question is a follow on from exercise 1-1, but this time looking at what the compiler does when an invalid escape sequence is passed to the printf function and the program is compiled.

```
/* Exercise 1-2. Experiment to find out what happens when printf's argument
 * string contains \c, where c is some character not listed above */

/* The reference to "not listed above" refers to the chapters introduction
 * of escape characters such as:
 * \n - Newline
 * \t - Tab
 * \b - Backspace
 * \\ - Backslash escape
*/

// hello.c

#include <stdio.h>

main ()
{
        printf("hello, world\k");
        // The \k in the statement is not a valid escape character

}


```

When this program is compiled,  the compiler will warn that the escape sequence is unknown. 

![](/Exercises/Images/invalid_escape_seq_complier_warn.png)

Since the program only causes a warning and not an error, the program can still be run as shown below. This still has an undersired affect, as the `\` is removed but the `k` remains after the string `hello, world`.

![](/Exercises/Images/invalid_escape_seq_compiles_and_runs.png)


