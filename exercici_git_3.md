Exercici GIT 3: Desfer canvis

Exercici 1

**1.** Elimina l\'última línia del fitxer index.txt i guarda-ho.

nano index.txt

\> ~~Capítol 5: Conceptes avançats~~

**2.** Comprova l\'estat del repositori.

git status

**3.** Desfés els canvis realitzats al fitxer index.txt per tornar a la
versió anterior del fitxer.

git restore index.txt

**4.** Torna a comprovar l\'estat del repositori.

git status

Exercici 2

**1.** Elimina l\'última línia del fitxer index.txt i guarda-ho.

nano index.txt

\> ~~Capítol 5: Conceptes avançats~~

**2.** Afegeix els canvis a la zona d\'intercanvi temporal.

git add index.txt

**3.** Comprova de nou l\'estat del repositori.

git status

**4.** Treu els canvis de la zona d\'intercanvi temporal, però
mantín-los al directori de treball.

git restore \--staged index.txt

**5.** Comprova de nou l\'estat del repositori.

git status

**6.** Desfés els canvis realitzats al fitxer index.txt per tornar a la
versió anterior del fitxer.

git restore index.txt

**7.** Torna a comprovar l\'estat del repositori.

git status

Exercici 3

**1.** Elimina l\'última línia del fitxer index.txt i guardar-ho.

nano index.txt

\> ~~Capítol 5: Conceptes avançats~~

**2.** Elimina el fitxer capítols/capitol3.txt.

rm capítols/capitol3.txt

**3.** Afegeix un fitxer nou capítols/capitol4.txt buit.

nano capítols/capitol4.txt

\> Capítol 4

**4.** Afegeix els canvis a la zona d\'intercanvi temporal.

git add \*

**5.** Comprova de nou l\'estat del repositori.

git status

**6.** Treu els canvis de la zona d\'intercanvi temporal, però
mantín-los al directori de treball.

git restore \--staged \*

**7.** Comprova de nou l\'estat del repositori.

git status

**8.** Desfés els canvis realitzats per tornar a la versió del
repositori.

git restore \*

**9.** Torna a comprovar l\'estat del repositori.

git status

Exercici 4

**1.** Elimina l\'última línia del fitxer index.txt i guardar-ho.

nano index.txt

\> ~~Capítol 5: Conceptes avançats~~

**2.** Elimina el fitxer capítols/capitol3.txt.

rm capítols/capitol3.txt

**3.** Afegeix els canvis a la zona d\'intercanvi temporal i fer un
commit amb el missatge \"Borrat accidental.\"

git add \*

git commit -m "Borrat accidental"

**4.** Comprova l\'historial del repositori.

git log \--oneline

**5.** Desfés l\'últim commit, però mantín els canvis anteriors al
directori de treball i a la zona d\'intercanvi temporal.

git reset \--soft HEAD\~1

**6.** Comprova l\'historial i l\'estat del repositori.

git log \--oneline

git status

**7.** Torna a fer el commit amb el mateix missatge d\'abans.

git commit -m "Borrat accidental"

**8.** Desfés l\'últim commit i els canvis anteriors al directori de
treball, tornant a la versió anterior del repositori.

git reset \--hard HEAD\~1

**9.** Comprova de nou l\'historial i l\'estat del repositori.

git log \--oneline\|git status
