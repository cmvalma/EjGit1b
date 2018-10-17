# CONFLICT IN GIT

* Read part 1 for previous iteration of the process in Windows; is is much more detailed and provides context for this one...

Now in Ubuntu, deleting .git folders work as expected. 

## PREPARAR ARCHIVOS
Crear folder específico con `mkdir`
### Iniciar Git 
`cd ExGit1`
`git init` 

### Crear archivos
touch 2_Readme.md`

IMG1
<img src="../EjGit1b/Pictures/IMG1.png"> 
      

El archivo conflictivo de Python se puede crear igual, pero lo creamos abriendo la carpeta ExGit1 y creando ahí el archivo "ConflictingFile.py"

## GESTIONAR GIT CONTROL
### Traer a escena todos los archivos:
`git add .`
IMG2
### Set defatult identity:
`git config -- global user.email "cmvalma.rg@gmail.com"`
`git config --global user.name "cmvalma"`
### Commit:
`git commit -m "primera version`
IMG3

## GITHUB 
Primero crear repositorio en Github 
### Añade el master al repo
**Conectar:** 
 `git remote add origin https://github.com/cmvalma/ExGit1.git`
Ne confundí, esta era la anterior. Para cambiar de dirección:
`https://github.com/cmvalma/ExGit1.gitgit remote set-url origin  https://github.com/cmvalma/EjGit1b.git`
**Push:**
`git push -u origin master`
IMG4

## BRANCH CON ARCHIVO MODIFICADO

IMG5
`git push --set-upstream origin Branch1`:
IMG6

## MERGE 
### Volvemos al Master
`git checkout master`
### y fusionamos la rama en él
`git merge Branch1`
Tampoco aparece el conflicto!! 
IMG7
