<h1 align ="center"> Hsh - Simple Shell</h1>
<hr/>
<h1 align ="center">
<img src="https://i.postimg.cc/8chZ4K8N/shell.jpg" height="80%" width="80%">
</h1>
<hr/>
<h1> Overview </h1>
<p>This is a simple, command-line implementation of the UNIX command line shell as part of our path and adventure in low-level programming and algorithms at Holberton School.</p>

<h2> Getting Started </h2>

<p> Clone this repository:</p>

```
git clone git@github.com:aaronJau21/holbertonschool-simple_shell.git
```

<p> Compile with</p>

```
<b>gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o *hsh</b>
```
```
./hsh
```
<p>Returns: 0 upon success or exit status upon error.</p>

<h2> Use </h2>
<p>After compiling the program, you can use it in both interactive and non-interactive mode.</p>

<h3> Interactive Mode </h3>
<ul>
<li>From the command line, enter "./" , followed by the executable name (ex: "./a.out").</li>
<li>After the "$ " prompt appears, type in a command to be executed. Repeat as desired.</li>
<li>To exit the program, you can type in either crtl + d or "exit".</li>
</ul>
<h3> Non - Interactive Mode </h3>
<ul>
<li>From the command line, use echo to pipe a command into the shell. Here's an example:</li>
</ul>

```
echo "pwd" | ./a.out
```
<table>
  <tr>
    <th>Command</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>env</td>
    <td>prints the environment</td>
  </tr>
  <tr>
    <td>exit</td>
    <td>exits out of our shell program</td>
  </tr>
</table>

<h2> Example Usage </h2>
<li>
<b>ls -l</b>   lists directory contents using a long listing format.
</li>

```
$ ls -l /tmp/
total 0
```

<li>
<b>pwd</b>   prints the working directory.
</li>

```
$ pwd
/home/vagrant/shelltesting
```

<li>
<b>fakefile</b>   prints error because "fakefile" does not exist
</li>

```
$ fakefile
fakefile: No such file or directory
```

<h2> Files </h2>
<table>
  <tr>
    <th>File Name</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>shell.c</td>
    <td>The main function, which calls other major functions for shell.</td>
  </tr>
  <tr>
    <td>programflowhelpers.c</td>
    <td>Major helper functions for shell (prompt, read user input, concatenate string for execve, fork, execute).</td>
  </tr>
  <tr>
    <td>stringhelpers.c</td>
    <td>Helper functions for reading and manipulating strings.</td>
  </tr>
  <tr>
    <td>tokenize+PATHhelpers.c</td>
    <td>Functions for tokenizing user input and handling the PATH.</td>
  </tr>
  <tr>
    <td>otherhelpers.c</td>
    <td>Other helper functions for strings and env built-in.</td>
  </tr>
  <tr>
    <td>holberton.h</td>
    <td>Header file with function prototypes, variables, and libraries.</td>
  </tr>
</table>
<h2> About </h2>
<p> Created on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89 </p>

# Authors
[<img src="https://avatars.githubusercontent.com/u/101225802?v=4" width=100><br><sub>Aaron Jauregui</sub>](https://github.com/aaronJau21) |  [<img src="https://avatars.githubusercontent.com/u/69946309?v=4" width=100><br><sub>Franco Cardenas </sub>](https://github.com/gustavofranco26) |
| :---: | :---: |
