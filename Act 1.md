Exercici 1
=
  
  Crea un repositori nou amb el nom llibre i mostra el seu contingut.
  Configura Git definint el nom de l'usuari, el correu electrònic i activa l'exida en color. Mostra la configuració final.
  
    - git config --global user.name "Nou Usuari"
    
    - git config --global user.email "correu@exemple.com"
    
    - git config --global color.ui true
    
    - git config --list    

Exercici 2
=

  Comprova l'estat del repositori.
  Crea un fitxer índex.txt amb el següent contingut:
  Comprova de nou l'estat del repositori.
  Afegeix el fitxer a la zona d'intercanvi temporal.
  Torna a comprovar una vegada més l'estat del repositori.
  
    - echo "Capitol 1: Introduix a git" > index.txt
    
    - echo "Capitol 2: Fluxe de treball basic" > index.txt
    
    - echo "Capitol 3: Repositoris Remots" > index.txt
    
    - git status

Exercici 3
=

  Realitza un commit dels últims canvis amb el missatge "Afegit índex del llibre." i revisa l'estat del repositori.
  
    - git commit -m "afegit index del llibre"
  
Exercici 4
=

  Canvia el fitxer índex.txt perquè continga el següent:
  Mostra els canvis respecte a l'última versió guardada al repositori.
  Fes un commit dels canvis amb el missatge "Afegit capítol 3 sobre gestió de branques".  
  
    - echo "Nou contingut del capitol 3" > index.txt
    
    - git diff
    
    - git add index.txt
    
    - git commit -m "Afegix capitol 3 sobre gestio de branques" 

Exercici 5
=

  Mostra els canvis de l'última versió del repositori respecte a l'anterior.
  Canvia el missatge de l'últim commit a "Afegit capítol 3 sobre gestió de branques a l'índex."
  Torna a mostrar els últims canvis del repositori.
  
    - git log -p
    
    - git commit --amend -m "Afegix capitol 3 sobre gestio de branques a l'index"
    
    - git log -p

Exercici 6
=

Indica a Git que vols ignorar tots els fitxers que comencen per "daw", tots els que tenen l'extensió out i les imatges (jpg, png, bmp i gif).

  - sudo nano .gitignore
