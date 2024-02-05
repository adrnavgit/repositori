Exercici GIT 4: Gestió de branques

Exercici 1

Crea una nova branca bibliografia i mostrar les branques del repositori.

git branch bibliografia

git branch

Exercici 2

**1.** Crear el fitxer capítols/capitol4.txt

cd capítols/

nano capitol4.txt

\> En aquest capítol veurem com utilitzar GitHub per allotjar
repositoris en remot.

**2.** Afegir els canvis a la zona d\'intercanvi temporal.

cd ..

git add capítols/capitol4.txt

**3.** Fer un commit amb el missatge \"Afegit capítol 4.\"

git commit -m "Afegit capítol 4"

**4.** Mostrar la història del repositori incloent totes les branques.

git branch -av

Exercici 3

**1.** Canvia a la branca bibliografia.

git checkout bibliografia

**2.** Crea el fitxer bibliografia.txt:

nano bibliografia.txt

\> - Chacon, S. and Straub, B. Pro Git. Apress

**3.** Afegeix els canvis a la zona d\'intercanvi temporal.

git add bibliografia.txt

**4.** Fes un commit amb el missatge \"Afegida primera referència
bibliogràfica\".

git commit -m \"Afegida primera referència bibliogràfica\"

**5.** Mostra la història del repositori incloent totes les branques.

git branch -av

Exercici 4

**1.** Fusiona la branca bibliografia amb la branca master.

git merge master

**2.** Mostra la història del repositori incloent totes les branques.

git branch -av

**3.** Elimina la branca bibliografia.

git checkout master

git branch -d bibliografia

**4.** Mostra de nou la història del repositori incloent totes les
branques.

git branch -av

Exercici 5

**1.** Crea la branca bibliografia.

git branch bibliografia

**2.** Canvia a la branca bibliografia.

git checkout bibliografia

**3.** Canvia el fitxer bibliografia.txt perquè continga les següents
referències:

nano bibliografia.txt

\> - Scott Chacon Ben Straub. Pro Git. Apress

\> - Ryan Hodson. Ry\'s Git Tutorial. Smashwords (2014)

**4.** Afegeix els canvis a la zona d\'intercanvi temporal i fer un
commit amb el missatge \"Afegida nova referència bibliogràfica.\"

git add bibliografia.txt

git commit -m "Afegida nova referència bibliogràfica"

**5.** Canvia a la branca master.

git checkout master

**6.** Canvia el fitxer bibliografia.txt perquè continga les següents
referències:

nano bibliografia.txt

\> - Chacon, S. and Straub, B. Pro Git. Apress

\> - Loeliger, J. and McCullough, M. Version control with Git. O\'Reilly

**7.** Afegeix els canvis a la zona d\'intercanvi temporal i fer un
commit amb el missatge \"Afegida nova referència bibliogràfica.\"

git commit -m "Afegida nova referència bibliogràfica"

**8.** Fusiona la branca bibliografia amb la branca master.

git checkout bibliografia

git merge master

**9.** Resol el conflicte deixant el fitxer bibliografia.txt amb les
referències:

nano bibliografia.txt

\> - Chacon, S. and Straub, B. Pro Git. Apress

\> - Loeliger, J. and McCullough, M. Version control with Git. O\'Reilly

\> - Hodson, R. Ry's Git Tutorial. Smashwords (2014)

**10.** Afegeix els canvis a la zona d\'intercanvi temporal i fes un
commit amb el missatge \"Resolt conflicte de bibliografia.\"

git add bibliografia.txt

git commit -m "Resolt conflicte de bibliografia"

**11.** Mostra la història del repositori incloent totes les branques.

git branch -av
