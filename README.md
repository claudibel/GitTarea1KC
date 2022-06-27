# GitTarea1KC
Práctica del curso de git, gitHub y Sourcetree

# Ejercicio 1

### ¿Qué comando utilizaste en el paso 11? ¿Por qué?
Emplee el comando `“git reset --hard HEAD~1”` ya que con este comando podemos deshacer el ultimo commit y lo que había en el working copy de manera que todo queda como estaba antes.   

### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Considero que se puede usar el comando `“git reset --hard HEAD~1”` este va a mover la rama al momento en que tuvo la iteración anterior. Aunque en mi caso use el comando “git reflog” que va apuntando los commits y una vez que los enliste podemos obtener el id del comitt (34d81ca) al cual deseamos volver y luego poder hacer un “git reset –hard b19729f” 

### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No se muestra ningún conflicto porque la rama styled tenía todos los cambios de la master

### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Si hay un conflicto “CONFLICT (content): Merge conflict in git-nuestro.md
Automatic merge failed; fix conflicts and then commit the result.” Esto ocasionado porque en ambas ramas hemos modificado las mismas líneas con respecto a la rama principal master.

Podemos ver con cat git-nuestro.md y ver las diferencias y solventarlas manualmente editando el archivo git-nuestro.md
https://www.atlassian.com/es/git/tutorials/using-branches/merge-conflicts

$ git add git-nuestro.md
$ git commit git-nuestro.md -m "20. Resolviendo conflicto merge"


### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No causo ningún conflicto. Porque cuando absorbe master a styled lo que hace es solo actualizar el archivo git-nuestro.cmd

### ¿Qué comando o comandos utilizaste en el paso 25?
Para visualizarlo use el comando `git log -graph`

### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Hacer un merge “no fast-forward” de “title” en “master” use el comando `“git merge –no-ff title”`. Y si pudo ser un fast forward ya que no hay ninguna ramificación desde el commit donde se hace el merge

### ¿Qué comando o comandos utilizaste en el paso 27?
Use el comando `git reset HEAD~1` ya que este comando permite deshacer el ultimo commit pero mantienen lo que había antes en el working copy. Solo el staging área quedaría vacio.

### ¿Qué comando o comandos utilizaste en el paso 28?
Use el comando `git checkout git-nuestro.md` pra volverlo al estado inicial

### ¿Qué comando o comandos utilizaste en el paso 29?
Primero asegurar de estar en otra rama diferente a title y luego ejecute el comando `git branch -D title`

### ¿Qué comando o comandos utilizaste en el paso 30?
En mi caso use `git reset –hard HEAD~1` porque deshacer el merge fue lo ultimo que habíamos realizado aunque también se pudo hacer ejecutando primero  “git reflog” y asi obtener el id del commit en el que hicimos el merge “no fast-forward” 

### ¿Qué comando o comandos usaste en el paso 32?
Para volver a situar a master en el commit inicial cuando se creó el poema primero reviso con el comando `“git reflog”` para obtener el id del commit y ya con el id del commit obtenido hago `“git reset id_commit`
En mi caso `git reset f3233daecd20e8ecf8bd7ceacf1b6fbac1e625cf`


### ¿Qué comando o comandos usaste en el punto 33?
git reflog para obtener el id del commit y luego un git reset –hard id_commit
`“$ git reset --hard 67cc324”`

### No he podido realizar la parte de etiquetas
