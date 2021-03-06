# RESOLUCIÓN DE CONFLICTO EN GIT
## CREACIÓN DE REPOSITORIO
Creamos también los archivos y el repositorio con los que generar el conflicto. 

### Crear directorio e inicializar Git. 

![i1](Pictures/i1.png)

![i2](Pictures/i2.png)

### Crear archivo .py "original" en el directorio. 

El código incluye la palabra original para diferenciarlo - cambiaremos esa palabra al menos

''*'' Lo había creado previamente en otra carpeta que había dado problemas, y 

`git con rm -rf .git`  

no consigue borrar el archivo .git oculto. Así que lo corto y pego en la carpeta master local. Como aún no he añadido (add nada), pienso que puede funcionar.   

![i3](Pictures/i3.png)

Por Bash:

![i4](Pictures/i4.png)

### Crear repositorio en GitHub 
Es más fácil que crearlo localmente desde el Bash. Una vez creado muestra el link y más información de ayuda. No es necesario que tengan el mismo nombre la carpeta local y el repositorio en GitHub:

![i5](Pictures/i5.png)

# RESOLUCIÓN DE CONFLICTO EN GIT -2 
## CONTROL DE VERSIONES
### Link carpeta local - GitHub
`git remote add origin https://github.com/thinktwise/tempProy1.git`

![i6](Pictures/i6.png)

**### Escenificar**

Añadir los cambios a escena. El punto tras add (o ./), añade todos los arhivos:

 ![i7](Pictures/i7.png)



**### Commit the new files

![i8](Pictures/i8.png)

Si no pongo la -m, abre un documento para hacer comentarios en vsCode. Git espera a que se cierre vsCode (todo el editor vsCode, no sólo los archivos) para continuar. 

**### push master al origen**

`git push -u origin master`

Pide **logear** en ventana pop:

![i9](Pictures/i9.png)



Si no entra a la primera, por alguna razón la vuelve a pedir con otro formato así:

![i10](Pictures/i10.png)

Al reconocer los datos, termina de crear la rama master:

![i11](Pictures/i11.png)



**## GENERACIÓN DE CAMBIOS CONFLICTIVOS**

**### Crear la nueva rama con el conflicto y cambiar a ella.**

con -b la crea nueva, además de cambiar el "foco" (i.e. situarse) en ella. 

![i12](Pictures/i12.png)

**### Alterar la línea de código**

En vez de original, ahora pone modified.

![i13](Pictures/i13.png)

**### commit el archivo modificado**

![i14](Pictures/i14.png)

**### Push la nueva rama**

![i15](Pictures/i15.png)



### Volver a master y unirla (merge) con la conflictiva

![i16](Pictures/i16.png)

**### Y... tacháaan: No encuentra conflicto!** 

A pesar de ser la misma línea la que se ha modificado, y solo una o dos palabras! Quizás porque no se creó el archivo originalmente el archivo en la carpeta de git y lo arrastré? Aunque después se escenificó con add... pero qué otra cosa podría ser?

Continuará... 

\- ver archivo 2_Readme.md

 
