Creo la carpeta cod_ramas_v1 en mi escritorio y me sitúo en ella:
cd desktop
mkdir cod_ramas_v1
cd cod_ramas_v1

Inicializo el repositorio cod_ramas_v1:
git init

Creo un archivo en java para la clase principal:
touch ClasePrincipal.java

Hago un commit de los cambios (commit A):
git add ClasePrincipal.java
git -m "Commit A, clase principal creada"

Subo los cambios en ClasePrincipal y hago el commit de ellos (commit B):
git add ClasePrincipal.java
git -m "Commit B, edito la clase principal"

Creo la rama 'exp' y navego hasta ella:
git checkout -b exp

Creo un archivo para la nueva clase:
touch ClaseExp.java

Hago un commit de los cambios (commit C):
git add ClaseExp.java
git commit -m "Commit C: creo la clase Exp"

Modifico la clase Exp y hago otro commit (commit D):
git add ClaseExp.java
git commit -m "Commit D: edito la clase Exp"

Vuelvo a la rama principal:
git checkout master

Modifico la clase principal por 2ª vez y hago commit:
git add ClasePrincipal.java
git commit -m "Commit E: edito por 2ª vez la clase principal"

Modifico la clase principal por 3ª vez y hago commit:
git add ClasePrincipal.java
git commit -m "Commit D: edito por 3ª vez la clase principal"

Hago un merge de la rama Exp en la rama principal:
git merge exp
