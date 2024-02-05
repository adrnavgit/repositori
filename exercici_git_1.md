**EXERCICIS DE CREACIÓ I ACTUALITZACIÓ DE REPOSITORIS**
=

**Exercici 1**
-

**1.** Crear un repositori nou amb el nom llibre i mostrar el seu contingut.

git init llibre

ll


**2.** Configurar Git definint el nom de l'usuari, el correu electrònic i activar l'eixida en color. Mostrar la configuració final.

Nom d'usuari: git config --global user.name "adrnavgit"

Correu electrònic: git config --global user.email "adrianavarroiev\@gmail.com"

Color: git config --global color.ui auto


**Exercici 2**
-

**1.** Comprovar l'estat del repositori.

git status

**2.** Crear un fitxer index.txt.

nano index.txt

**3.** Comprovar de nou.

git status

**4.** Afegir el fitxer a la zona d'intercanvi temporal.

git add index.txt

**5.** Tornar a comprovar l'estat.

git status


**Exercici 3**
-

Realitzar un commit amb el missatge "Afegint índex del llibre".

git commit -m "Afegint índex del llibre"

Veure l'estat del repositori.

git status


**Exercici 4**
-

**1.** Canviar el fitxer index.txt.

nano index.txt

**2.** Mostrar els canvis.

git status

**3.** Fer un commit amb el missatge "Afegit capítol 3 sobre gestió de branques".

git commit -m "Afegit capítol 3 sobre gestió de branques"


**Exercici 5**
-

**1.** Mostrar canvis.

git status

**2.** Canviar el missatge de l'últim commit.

Desfer el commit: git reset --soft HEAD~

git commit -m "Afegit capítol 3 sobre gestió de branques a l'índex"

**3.** Tornar a mostrar els canvis.

git status


**Exercici 6**

Ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out, jpg, png, bmp i gif.

nano .gitignore

#Fitxers ignorats

daw*

*.out

#Imatges

*.jpg

*.png

*.bmp

*.gif

git add .gitignore

git commit -m "Afegint fitxer .gitignore"
