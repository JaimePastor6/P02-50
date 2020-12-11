# P02-50
 Creamos una nueva rama con git branch "NombreDeLaRama" y cambiamos de rama con git checkout "NombreDeLaRama"
 Hacemos los cambios en la rama creada y los subimos, git push "url"
 Cambiamos a la rama principal, hacemos un cambio y lo subimos, nos dara error (Fetch first)
 Ponemos:
    -git fetch origin main:tmp
    -git rebase tmp
    -git push origin HEAD:main
 Y luego git log --graph --oneline --decorate --all para ver el grafico, que nos da como resultado:
 
* bdaf332 (HEAD -> main, origin/main, origin/HEAD) Cambios en la rama principal
| * 07c5d8e (rama) Cambio desde otra rama
|/
* 1174f0d Update README.md
* ef378dc Add files via upload
* 98bbcf0 Initial commit
* 35624c2 (tag: V1.0) Update README.md
* a153954 Cambio desde CarpetaInstituto
* ec4d7c7 Cambio desde CarpetaCasa
* 2d94b5f Cambio local
* 2e204d3 Add files via upload
* effe2d3 Initial commit
