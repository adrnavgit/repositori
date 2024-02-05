EXERCICIS DE CREACIÓ I ACTUALITZACIÓ DE REPOSITORIS

Exercici 1

**1.** Crear un repositori nou amb el nom llibre i mostrar el seu
contingut.

![](Pictures/10000000000002DF000001D00816FE477FC2C3A3.png){width="17cm"
height="10.732cm"}

**2.** Configurar Git definint el nom de l\'usuari, el correu electrònic
i activar l\'eixida en color. Mostrar la configuració final.

![](Pictures/1000000000000314000000D860A789F5D028E73D.png){width="17cm"
height="4.658cm"}

\- Nom d'usuari: git config \--global user.name "adrnavgit"

\- Correu electrònic: git config \--global user.email
"adrianavarroiev\@gmail.com"

\- Color: git config \--global color.ui auto

Exercici 2

**1.** Comprovar l'estat del repositori.

git status

**2.** Crear un fitxer index.txt.

nano index.txt

**3.** Comprovar de nou.

git status

![](Pictures/1000000000000337000001D4FBAAEB535EDE5DEE.png){width="17cm"
height="9.666cm"}

**4.** Afegir el fitxer a la zona d'intercanvi temporal.

git add index.txt

**5.** Tornar a comprovar l'estat.

git status

![](Pictures/100000000000026D000000FBB6E7F12FD7820E64.png){width="16.431cm"
height="6.641cm"}

Exercici 3

Realitzar un commit amb el missatge "Afegint índex del llibre".

git commit -m "Afegint índex del llibre"

Veure l'estat del repositori.

git commit

![](Pictures/100000000000034B000000C695BA56214C5B2EFD.png){width="17cm"
height="3.992cm"}

Exercici 4

**1.** Canviar el fitxer index.txt.

nano index.txt

**2.** Mostrar els canvis.

git status

**3.** Fer un commit amb el missatge "Afegit capítol 3 sobre gestió de
branques".

git commit -m "Afegit capítol 3 sobre gestió de branques"

![](Pictures/100000000000036D000001AE31D0F7B1D5B97628.png){width="17cm"
height="8.334cm"}

Exercici 5

**1.** Mostrar canvis.

git status

**2.** Canviar el missatge de l'últim commit.

Desfer el commit: git reset \--soft HEAD\~

git commit -m "Afegit capítol 3 sobre gestió de branques a l\'índex"

**3.** Tornar a mostrar els canvis.

git status

![](Pictures/10000000000002F800000177F968C9C85E38A481.png){width="17cm"
height="8.387cm"}

Exercici 6

Ignorar tots els fitxers que comencen per "daw", tots els que tenen
l'extensió out, jpg, png, bmp i gif.

nano .gitignore

\#Fitxers ignorats

daw\*

\*.out

\#Imatges

\*.jpg

\*.png

\*.bmp

\*.gif

git add .gitignore

![](Pictures/1000000000000258000000FA3CC7A898871DE656.png){width="15.875cm"
height="6.615cm"}git commit -m "Afegint fitxer .gitignore"
