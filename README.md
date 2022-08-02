<h1 align ="center"> Hsh - Simple Shell</h1>
<hr/>
<h1 align ="center">
<img src="https://i.postimg.cc/8chZ4K8N/shell.jpg" height="80%" width="80%">
</h1>
<hr/>
<h1> Overview </h1>
<p>This is a simple, command-line implementation of the UNIX command line shell as part of our path and adventure in low-level programming and algorithms at Holberton School.</p>

<h2> Getting Started </h2>

<p> Clone this repository: git clone [Link Repository]. </p>
<p> Compile with <b>gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o *hsh</b> </p>
<p>./hsh</p>
<p>Returns: 0 upon success or exit status upon error.</p>

<h2> Usage </h2>
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
<tr><th>Command</th><th>Description</th></tr>
<tr><th>env</th><th>prints the environment</th></tr>
<tr><th>exit</th><th>exits out of our shell program</th></tr>
</table>

# Authors
[<img src="https://avatars.githubusercontent.com/u/101225802?v=4" width=100><br><sub>Aaron Jauregui</sub>](https://github.com/aaronJau21) |  [<img src="https://avatars.githubusercontent.com/u/69946309?v=4" width=100><br><sub>Franco Cardenas </sub>](https://github.com/gustavofranco26) |
| :---: | :---: |
