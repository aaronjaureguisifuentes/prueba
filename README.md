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
Visión general
Este es un intérprete de línea de comandos de UNIX basado en el shell simple (sh). Lee la entrada del usuario desde la línea de comandos, la interpreta y ejecuta los comandos.

Empezando
Clona este repositorio. Compile con GCC y use las siguientes banderas: gcc -Wall -Werror -Wextra -pedantic

Devuelve: 0 en caso de éxito o estado de salida en caso de error

Uso
Después de compilar el programa, puede usarlo tanto en modo interactivo como no interactivo.

Modo interactivo
Desde la línea de comando, ingrese "./", seguido del nombre del ejecutable (por ejemplo: "./a.out").
Después de que aparezca el indicador "$", escriba un comando para ejecutarlo. Repita según lo desee.
Para salir del programa, puede escribir crtl + d o "salir".
Modo no interactivo
Desde la línea de comando, use echo para canalizar un comando al shell. Aquí hay un ejemplo:
echo "pwd" | ./a.out
Integraciones de Simple_Shell
Dominio	Descripción
env	imprime el medio ambiente
salida	sale de nuestro programa shell
Ejemplo de uso
ls -l enumera los contenidos del directorio utilizando un formato de listado largo
$ ls -l /tmp/
total 0
pwd imprime el directorio de trabajo
$ pwd
/home/vagrant/shelltesting
fakefile imprime error porque "fakefile" no existe
$ fakefile
fakefile: No such file or directory
archivos
Nombre del archivo	Descripción
shell.c	la función principal, que llama a otras funciones principales para shell
programflowhelpers.c	principales funciones auxiliares para shell (indicar, leer la entrada del usuario, concatenar cadena para execve, bifurcar, ejecutar)
stringhelpers.c	funciones auxiliares para leer y manipular cadenas
tokenize+PATHhelpers.c	funciones para tokenizar la entrada del usuario y manejar la RUTA
otherhelpers.c	otras funciones auxiliares para cadenas y env incorporadas
holberton.h	Archivo de encabezado con prototipos de funciones, variables y bibliotecas
Sobre
Creado el Ubuntu 14.04 LTS. Compilado con gcc 4.8.4, usando banderas:-Wall -Werror -Wextra and -pedantic
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

# Authors
| [<img src="https://avatars.githubusercontent.com/u/101225802?v=4" width=100><br><sub>Aaron Jauregui</sub>](https://github.com/aaronJau21) |  [<img src="https://avatars.githubusercontent.com/u/69946309?v=4" width=100><br><sub>Franco Cardenas </sub>](https://github.com/gustavofranco26) |
| :---: | :---: |
