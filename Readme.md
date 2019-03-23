# CONFLICT IN GIT

*Note: Read "Pre-Readme" for previous iteration of the process in Windows; it is much more detailed and provides context for this Readme.

Contrary to previous iterations of the process in Windows, in Ubuntu, deleting .git folders works as expected.

## PREPARAR ARCHIVOS
Crear folder específico con `mkdir`
### Iniciar Git 
`cd ExGit1`
`git init` 

### Crear archivos
touch 2_Readme.md`

<img src="/Pictures/IMG1.png"/> 
      

El archivo conflictivo de Python se puede crear igual, pero lo creamos abriendo la carpeta ExGit1 y creando ahí el archivo "ConflictingFile.py"

## GESTIONAR GIT CONTROL
### Traer a escena todos los archivos:
`git add .`

<img src="/Pictures/IMG2.png"/> 
### Set defatult identity:
`git config -- global user.email "cmvalma.rg@gmail.com"`
`git config --global user.name "cmvalma"`
### Commit:
`git commit -m "primera version`
<img src="/Pictures/IMG3.png"/> 

## GITHUB 
Primero crear repositorio en Github 
### Añade el master al repo
**Conectar:** 
 `git remote add origin https://github.com/cmvalma/ExGit1.git`
Ne confundí, esta era la anterior. Para cambiar de dirección:
`https://github.com/cmvalma/ExGit1.gitgit remote set-url origin  https://github.com/cmvalma/EjGit1b.git`
**Push:**
`git push -u origin master`
<img src="/Pictures/IMG4.png"/> 

## BRANCH CON ARCHIVO MODIFICADOInsightAfterAddingPicsinGitHub.png

<img src="/Pictures/IMG5.png"/> 
`git push --set-upstream origin Branch1`:
<img src="/Pictures/IMG6.png"/> 

## MERGE 
### Volvemos al Master
`git checkout master`
### y fusionamos la rama en él
`git merge Branch1`
Tampoco aparece el conflicto!! 
<img src="/Pictures/IMG7.png"/> 

## INSIGHT SCREENSHOTS

<img src="/Pictures/Insight1.png"/>
      
Despues de añadir las fotos directamente via GitHub : 

<img src="/Pictures/InsightAfterAddingPicsinGitHub.png"/>
