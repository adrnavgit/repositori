**Exercici GIT 2: Ús de l'historial de canvis**

**Exercici 1**
-

**1.** Mostra l'historial de canvis del repositori.

git status

**2.** Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt:

mkdir capítols

cd capítols/

nano capitol.txt

> Git és un sistema de control de versions ideat per Linus Torvalds.

**3.** Afegeix els canvis a la zona d'intercanvi temporal (staging area).

git add capitol1.txt

**4.** Fes un commit dels canvis amb el missatge "Afegit capítol 1".

git commit -m "Afegit capítol 1"

**5.** Torna a mostrar l'historial de canvis del repositori.

git status


**Exercici 2**
-

**1.** Crea el fitxer capitol2.txt a la carpeta capítols:

nano capitol2.txt

> El flux de treball bàsic amb Git consisteix en:

> 1- Fer canvis al repositori.

> 2- Afegir els canvis a la zona d'intercanvi temporal.

> 3- Fer un commit dels canvis

**2.** Afegeix els canvis a la zona d'intercanvi temporal.

git add capitol2.txt

**3.** Fes un commit dels canvis amb el missatge "Afegit capítol 2".

git commit -m "Afegit capítol 2"

**4.** Mostra les diferències entre l'última versió i les dues versions
anteriors.

git diff HEAD~2..HEAD


**Exercici 3**
-

**1.** Crea el fitxer capitol3.txt a la carpeta capítols amb el següent
text:

nano capitol3.txt

> Git permet la creació de branques, la qual cosa permet tindre distintes versions del mateix projecte i treballar simultàniament en elles.

**2.** Afegeix els canvis a la zona d'intercanvi temporal.

git add capitol3.txt

**3.** Fes un commit dels canvis amb el missatge "Afegit capítol 3".

git commit -m "Afegit capítol 3"

**4.** Mostra les diferències entre la primera i l'última versió del repositori.

Primer commit: 45a1e20

Últim commit: 931a696

git diff 45a1e20 931a696


**Exercici 4**
-

**1.** Afegir al final del fitxer index.txt la següent línia:

cd ..

nano index.txt

...

> Capítol 5: Conceptes avançats

**2.** Afegir els canvis a la zona d'intercanvi temporal.

git add index.txt

**3.** Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex".

git commit -m "Afegit capítol 5 a l'índex"

**4.** Mostrar qui ha fet canvis sobre el fitxer index.txt.

git log -- index.txt
