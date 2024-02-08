Exercici GIT 2: Ús de l'historial de canvis
=

Exercici 1
-

Mostra l'historial de canvis del repositori.
Crea la carpeta capítols i dins d'ella crea el fitxer capitol1.txt amb el següent text:

Afegeix els canvis a la zona d'intercanvi temporal (staging area)
Fes un commit dels canvis amb el missatge "Afegit capítol 1."
Torna a mostrar l'historial de canvis del repositori.

>git log
>
>mkdir capitols
>
>nano capitols/capitol1.txt
>
>git add capitols/capitol1.txt
>
>git commit -m “Afegit capitol 1”
>
>git log

Exercici 2
-

Crea el fitxer capitol2.txt a la carpeta capítols amb el següent text:

Afegeix els canvis a la zona d'intercanvi temporal.
Fes un commit dels canvis amb el missatge "Afegit capítol 2."
Mostra les diferències entre l'última versió i les dues versions anteriors.

>nano capitols/capitol2.txt
>
>git add capitols/capitol2.txt
>
>git commit -m “Afegit capitol 2”
>
>git diff HEAD~2..HEAD

Exercici 3
-

Crea el fitxer capitol3.txt a la carpeta capítols amb el següent text:

Afegeix els canvis a la zona d'intercanvi temporal.
Fes un commit dels canvis amb el missatge "Afegit capítol 3."
Mostra les diferències entre la primera i l'última versió del repositori.

>nano capitols/capitol3.txt
>
>git add capitols/capitol3.txt
>
>git commit -m “Afegit capitol 3”
>
>git diff HEAD~2..

Exercici 4
-

Afegir al final del fitxer índex.txt la següent línia:

Afegir els canvis a la zona d'intercanvi temporal.
Fer un commit dels canvis amb el missatge "Afegit capítol 5 a l'índex."
Mostrar qui ha fet canvis sobre el fitxer índex.txt.

>nano index.html (text necessari)
>
>git add index.html
>
>git commit -m “Afegit capitol 5 a l’index”
>
>git blame index.txt
