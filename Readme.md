# PRACTICA GITHUB - NICOLAS CABALLERO 

En esta practica responderemos las preguntas puestas en el ejercico 1 de la practica de Git. 

1. ¿Qué comando utilizaste en el paso 11? ¿Por qué? 
    * deshacer el ultimo commit
        * usamos el comando git reset --hard HEAD~1 para deshacer completamente los cambios hechos en el anterior commit perdiendo completamente los datos del commit en el que estabamos

2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
    * rehacer el ultimo commit
        * usamos el comando reflog para ver el identificador del commit anterior antes de que hicieramos el reset. despues de identificarlo usamos el comando reset --hard (id que vimos en reflog). despues veremos que la rama master y styled estan en un commit diferente
3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 
    * Hacer un merge con "master" 
        * No no ha causado conflictos porque a hacer el merge,git se ha dado cuenta que los unicos cambios del archivo git-nustro, son por simbolos en cada linea. si hubiese algo totalmente diferente podria dar un conflicto.
4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
    * hacer un merge de htmlify en styled 
        * no Ha dado ningun error porque en las lineas que ha cambiado se ha reemplzadado los signos por codigos que pueden ser lo mismo
5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
    * Hacer merge de master a Styled
        * No hizo conflicto por la misma razon de hacer merge con Styled y Htmlify 
6. ¿Qué comando o comandos utilizaste en el paso 25? 
7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 
8. ¿Qué comando o comandos utilizaste en el paso 27? 
9. ¿Qué comando o comandos utilizaste en el paso 28? 
10. ¿Qué comando o comandos utilizaste en el paso 29? 
11. ¿Qué comando o comandos utilizaste en el paso 30? 
12. ¿Qué comando o comandos usaste en el paso 32? 
13. ¿Qué comando o comandos usaste en el punto 33?