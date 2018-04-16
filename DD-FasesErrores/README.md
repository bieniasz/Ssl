. Autores de la resolución: Ezequiel Bieniasz.
Usuario github: bieniasz
Legajo: 1637782
Titulo:Trabajo numero 1 - Fases de traducción y Errores.
Objetivo:Identificar las fases de traducción y errores
hello2.c
>gcc -E -o hello2.i hello2.c

-Aparecen todas las declaraciones que son propias del #include <studio.h> y desaparecen los comentarios, los cuales son reemplazados por espacios

hello3.c
>gcc -E -o hello3.i hello3.c

-Podemos observar que aparecen seis lineas arriba de la declaración del printf.

>gcc -S hello3.i

-Al compilar aparece una señal de advertencia o tambien denominada warning que hace referencia a la función prontf y un error de declaracion o declaracipon esperada al final, haciendo referencia a que falta poner la llave de cierre.

Hello4.c 

>gcc -E -o hello4.i hello4.c

>gcc -S hello4.i

-Aparece un warning haciendo referencia a la función prontf

>gcc -E -o hello5.i hello5.c

>gcc -S hello5.i

-Aparece un warning haciendo referencia al formato de "%d", informando que espera un argumento del tipo int

>gcc -c hello5.s

>gcc -o hello5 hello5.o

-Al ejecutarlo aparece un número el cual puede variar, la salida que podemos ver es "basura" que estaba posicionada en esa posición de memoria.

hello6.c
>gcc -E -o hello6.i hello6.c

>gcc -S hello6.i

>gcc -c hello6.s

>gcc -o hello6 hello6.o

-No presenta errores, al ejecutar aparece el mensaje "La respuesta es 42"

hello7.c
>gcc -E -o hello7.i hello7.c

>gcc -S hello7.i

-Aparece un warning por no haber declarado la función printf, ademas podemos apreciar una nota en la que se incluye "<stdio.h>

>gcc -c hello7.s

>gcc -o hello7 hello7.o

-Al ejecutarlo aparece la nota "La respuesta es 42",sin ningun tipo de problemas.
Y por ultimo funciona sin haberla declarado por que el gcc compiler incluye por defecto la <stdio.h>
