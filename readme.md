 **1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

1. git reset HEAD ~1
2. 
git status y tenemos el archivo don-quijote.md modificado

Porque queríamos deshacer el último commit (perdiendo los cambios realizados en el working copy). 

**2.¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

1. git add don-quijote.md
2. Git commit –m “3 Parte”
3. Git log para comprobar si lo hemos hecho bien

Porque tenía que rehacer el último commit, el que acabábamos de deshacer. Y lo nombramos como "3 Parte" en vez del título anterior “Guardo los primeros cambios realizados en el archivo don-quijote.md” para no confundirnos. Y porque realmente lo que hemos guardado en el commit la acción de rehacer el último commit, y no es la misma acción que en el anterior commit, aunque el texto que contenga es el mismo.

**3. El merge del paso 13, ¿Causó algún conﬂicto? ¿Por qué?**

No, no me ha causado ningún conflicto, ya que ya estaba en la rama style para absorber a master.

**4.El merge del paso 19, ¿Causó algún conﬂicto? ¿Por qué?** 

No, pero porque antes había cambiado a la rama styled para poder absorber la rama htmlify

1. git checkout styled
2. git branch: para ver las ramas
3. git merge htmlify: styled absorbe a htmlify


**5.El merge del paso 21, ¿Causó algún conﬂicto? ¿Por qué?** 

No, pero la respuesta es igual que la anterior, porque antes cambiamos a la rama master para absorber la rama styled, que es donde estábamos en el paso anterior.

1. git checkout master
2. git merge styled


**6.¿Qué comando o comandos utilizaste en el paso 25?**

git graph

**7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí, porque realmente la rama title acababa de surgir de la rama master, es decir, solo habíamos creado un paso más que provenía directamente de master. Así que podría haber sido un fast forward ya que esta en la misma "línea".
 
**8.¿Qué comando o comandos utilizaste en el paso 27?**

git reset --soft HEAD~1

**9.¿Qué comando o comandos utilizaste en el paso 28?**

git reset --hard HEAD~1

**10.¿Qué comando o comandos utilizaste en el paso 29?**

git branch –D title

**11.¿Qué comando o comandos utilizaste en el paso 30?** 

1. git reflog : para ver el código del merge que queremos rehacer
2. Rehacer el merge: git reset --hard 03f4014


**12.¿Qué comando o comandos usaste en el paso 32?**

Para volver al commit inicial cuando se creó el poema utilicé los comandos:
 
1. git log: para ver el código del primero commit
2. git checkout d712930175: Estamos en el primer commit


**13.¿Qué comando o comandos usaste en el punto 33?**


1. git log: para ver el código del commit donde pusimos el título al poema
2. git checkout 03f40143e3d84e: Volvemos al commit “Añadimos título al texto”
