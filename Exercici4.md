Exercici GIT 4: Gestió de branques
=

Exercici 1
-

Crea una nova branca bibliografia i mostrar les branques del repositori.

>git branch bibliografia
>
>git branch

Exercici 2
-

Crear el fitxer capítols/capitol4.txt i afegir el següent text

Afegir els canvis a la zona d'intercanvi temporal.
Fer un commit amb el missatge "Afegit capítol 4."
Mostrar la història del repositori incloent totes les branques.

>nano capitols/capitol4.txt
>
>git add capitols/capitol4
>
>git commit -m “Afegit capitol 4”
>
>git log --all --decorate --oneline --graph

Exercici 3
-

Canvia a la branca bibliografia.
Crea el fitxer bibliografia.txt i afegir la següent referència:

Afegeix els canvis a la zona d'intercanvi temporal.
Fes un commit amb el missatge "Afegida primera referència bibliogràfica."
Mostra la història del repositori incloent totes les branques.

>git checkout bibliografia
>
>nano bibliografia.txt
>
>git add bibliografia.txt
>
>git commit -m “Afegida primera referència bibliogràfica”
>
>git log --all --decorate --oneline --graph

Exercici 4
-

Fusiona la branca bibliografia amb la branca master.
Mostra la història del repositori incloent totes les branques.
Elimina la branca bibliografia.
Mostra de nou la història del repositori incloent totes les branques.

>git checkout master
>
>git merge bibliografia
>
>git log --all --decorate --oneline –graph
>
>giti branch -d bibliografia
>
>git log --all --decorate --oneline --graph

Exercici 5
-

Crea la branca bibliografia.
Canvia a la branca bibliografia.
Canvia el fitxer bibliografia.txt perquè continga les següents referències:

Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."
Canvia a la branca master.
Canvia el fitxer bibliografia.txt perquè continga les següents referències:

Afegeix els canvis a la zona d'intercanvi temporal i fer un commit amb el missatge "Afegida nova referència bibliogràfica."
Fusiona la branca bibliografia amb la branca master.
Resol el conflicte deixant el fitxer bibliografia.txt amb les referències:

Afegeix els canvis a la zona d'intercanvi temporal i fes un commit amb el missatge "Resolt conflicte de bibliografia."
Mostra la història del repositori incloent totes les branques.

>git branch bibliografia
>
>git checkout bibliografia
>
>nano bibliografia.txt

>git add bibliografia.txt
>
>git commit -m “Afegida nova referència bibliogràfica”
>
>git checkout master
>
>nano bibliografia.txt
>
>git commit -m “Afegida nova referència bibliogràfica”
>
>git merge bibliografia
>
>git log --all --decorate --oneline --graph
