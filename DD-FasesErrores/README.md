. Autores de la resolución: Ezequiel Bieniasz.
Usuario github: bieniasz
Legajo: 1637782
Titulo:Trabajo numero 1 - Fases de traducción y Errores.
Objetivo:Identificar las fases de traducción y errores
1.  hello2.c
>gcc -E -o hello2.i hello2.c
Aparecen todas las declaraciones que son propias del #include <studio.h> y desaparecen los comentarios, los cuales son remplazados por espacios

2.hello3.c
>gcc -E -o hello3.i hello3.c
Podemos observar que aparecen seis lineas arriba de la declaración del printf.

3. >gcc -S hello3.i
Al compilar aparece una señal de advertencia o tambien denominada warning que hace referencia a la función prontf y un error de declaracion o declaracipon esperada al final, haciendo referencia a que falta poner la llave de cierre.

4.g
