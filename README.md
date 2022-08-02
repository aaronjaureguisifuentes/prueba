<h1>C - Simple Shell</h1>
<hr />
/*<h3>collaborators</h3>
<ol>
    <li>Aaron Jauregui </li>
    <li>Franco Cardenas </li>
</ol>

<h2>Description</h2>
<hr/>

<p>This is an implementation of a Unix shell interpreter interface.</p>
<small>the main objective of the project is to improve the understanding of the C language by collaborators, to become more familiar with the Unix Operating System, better called <b>Shell</b> so manage the greater complexity of the program </small>


<h2> What does our shell do? </h2>

<p>Is a command interpreter of an operating system </p>

<h3> Copilation and Usage </h3>
<p> git clone [Link Repository] </p>
<p> $gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o *hsh </p>
<p>./hsh</p>

<p>[Enter following the shell commands]</p>

<h3>Comands Description</h3>
<span> echo Holberton </span>
<p> In the above command, the echo command will write its Holberton argument to standard output.</p>
<p>Another command to execute in the hsh, in order to have a better interaction with the program, is the cd command, which allows us to change the directory and be able to view the different files that exist in it.</p>
<span>cd</span>
<p>In order to list the number of files that exist in our directory, we can use the following command:</p>
<span>ls</span>*/
<h1 align ="center">
<img src="https://i.postimg.cc/8chZ4K8N/shell.jpg" height="60%" width="50%">
</h1>
<a href="https://postimg.cc/4HxvN1NS" target="_blank"><img src="https://i.postimg.cc/4HxvN1NS/shell.jpg" alt="shell"/></a><br/><br/>
# Printf

# Synopsis
This is a simple implementation of printf function that formats and prints data

# Description
The _printf() function produces output according to a format which is described
below. This function write its output to the stdout, the standard output stream. Returns the count of printed characters when the function is successful and -1 when the function fails.

The available convertion specifiers are:
 %c: Prints a single character.
 %s: Prints a string of characters.
 %%: Prints percent.
 %d: Prints integers.
 %i: Prints integers.

# Usage
 All the files are to be compiled on Ubuntu 20.04 LTS
 Compile your code with "gcc -Wall -Werror -Wextra -pedantic -std=gnu89 -Wno-format *.c"
 Include the "main.h" header file on the functions using the _printf()

# Example

```
#include "main.h"
#include <limits.h>
#include <stdio.h>

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    int len;
    int len2;

    len = _printf("Let's try to printf a simple sentence.\n");
    len2 = printf("Let's try to printf a simple sentence.\n");
    _printf("Length:[%d, %i]\n", len, len);
    printf("Length:[%d, %i]\n", len2, len2);
    _printf("Negative:[%d]\n", -762534);
    printf("Negative:[%d]\n", -762534);
    _printf("Character:[%c]\n", 'H');
    printf("Character:[%c]\n", 'H');
    _printf("String:[%s]\n", "I am a string !");
    printf("String:[%s]\n", "I am a string !");
    len = _printf("Percent:[%%]\n");
    len2 = printf("Percent:[%%]\n");
    _printf("Len:[%d]\n", len);
    printf("Len:[%d]\n", len2);
    return (0);
}
```

# Autors
| [<img src="https://avatars.githubusercontent.com/u/101225802?v=4" width=100><br><sub>Aaron Jauregui</sub>](https://github.com/aaronJau21) |  [<img src="https://avatars.githubusercontent.com/u/69946309?v=4" width=100><br><sub>Franco Cardenas </sub>](https://github.com/gustavofranco26) |
| :---: | :---: |
