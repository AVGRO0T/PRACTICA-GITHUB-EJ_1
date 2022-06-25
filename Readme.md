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
	* Dibujar el diagrama
		* git log --graph
7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 
	* Hacer un merge “no fast-forward” de “title” en “master”
		* si, porque no cree un commit nuevo en la rama head que pueda ser un problema para perder ese commit. Si hubiese tenido mas commits en la rama Head me obligaria a hacer un merge no fast forward.
8. ¿Qué comando o comandos utilizaste en el paso 27? 
	* Deshacer el merge
		* git reset HEAD~1
9. ¿Qué comando o comandos utilizaste en el paso 28? 
	* Descartar los cambios
		* git restored git-nuestro.md
10. ¿Qué comando o comandos utilizaste en el paso 29? 
	* Eliminar la rama “title”
		* git branch -D title --> tengo que estar en otra rama con git checkout master
11. ¿Qué comando o comandos utilizaste en el paso 30? 
	* Rehacer el merge que hemos deshecho 
		* git reflog --> para ver el identificador del commit antes de deshacer el merge
		* git reset 0dbc150
		* git add git-nuestro --> porque aparecen cambios
		* git commit --> Para crear un nuevo commit que este sin el titulo y el merge se queda on el titulo
		* git reset --hard HEAD~1 --> restaura al merge de title y muestra el titulo
12. ¿Qué comando o comandos usaste en el paso 32? 
	* Volver al commit inicial cuando se creó el poema
		* git log --> para ver el hash del primer commit
		* git checkout <HASH del commit> 	
13. ¿Qué comando o comandos usaste en el punto 33?
	* Volver al estado final, cuando pusimos título al poema
		* git checkout Master --> que contiene todas las commits desde el inicio hasta el final dodne se encuentra ella