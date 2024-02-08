Exercici 1
=

  Crea una nova branca bibliografia i mostrar les branques del repositori.

    -echo "Fer un commit amb el missatge \"Afegix capitol 4."" > capitols/capitols4.txt > En aquest capitol veurem com utilitzar GitHubper allotja repositoris en remot

    -git add capitols/capitol4.txt

    -git commit - m "Afegix capitol 4."

    -git log --all --graph --decorate

Exercici 2
=

  Crear el fitxer capítols/capitol4.txt i afegir el següent text
  Afegir els canvis a la zona d'intercanvi temporal.
  Fer un commit amb el missatge "Afegit capítol 4."
  Mostrar la història del repositori incloent totes les branques.

    -git checkout -b bibliografia

    -echo "Afegix els canvis a la zona d'intercanvi temporal" > bibliografia.txt

    -echo Fer un commit amb el missatge \"Afegida primera referencia bibliografia.\"" >> bibliografia.txt

    -git add bibliografia.txt

    -git commit -m "Afegida primera referencia bibliografica"

    -git log --all --graph --decorate  

Exercici 3
=

  Canvia a la branca bibliografia.
  Crea el fitxer bibliografia.txt i afegir la següent referència:
  Afegeix els canvis a la zona d'intercanvi temporal.
  Fes un commit amb el missatge "Afegida primera referència bibliogràfica."
  Mostra la història del repositori incloent totes les branques.

    -git checkout master

    -git merge bibliografia

    -git log --all --graph --decorate

    -git branch -d bibliografia

    -git log --all --graph --decorate

Exercici 4
=

  Fusiona la branca bibliografia amb la branca master.
  Mostra la història del repositori incloent totes les branques.
  Elimina la branca bibliografia.
  Mostra de nou la història del repositori incloent totes les branques.

    -git checkout -b bibliografia

    -echo "Afegix els canvis a la zona d'intercanvi temporal." > bibliografia.txt

    -echo "Fer un commit amb el missatge \"Afegida nova referencia bibliografica.\"" >> bibliografia.txt

    -git add bibliografia.txt

    -git commit -m "Afegix nova referencia bibliografica"

    -git checkout master

    -echo "Afegix els canvis a la zona d'intercanvi temporal." > bibliografia.txt

    -echo "Fer un commit amb el missat \ "Afegida nova referencia bibliografica.\"" >> bibliografia.txt

    -git add bibliografia.txt

    -git merge bibliografia

    -git commit -m "Resol conflicte bibliografia"

Exercici 5
=

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

    -git branch bibliografia
    
    -git checkout bibliografia
    
    -echo "Nova referencia bibliografica A" > bibliografia.txt
    
    -echo "Nova referencia bibliografica B" > bibliografia.txt
    
    -git add bibliografia
    
    -git commit -m "Afegida nova referencia bibliografica"
    
    -git checkout master
    
    -echo "Nova referencia bibliografica X" > bibliografia.txt
    
    -echo "Nova referencia bibliografica Y" > bibliografia.txt
    
    -git add bibliografia
    
    -git commit -m "Afegida nova referencia bibliografica"
    
    -git merge bibliografia
