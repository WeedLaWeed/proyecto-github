# Pasos realizados para proyecto-github:
1) se creó un repositorio desde github online concreate repository

2) se clonó el repositorio en local con los siguientes comandos:
cd "C:\Users\User\Documents\GitHub"
git clone https://github.com/WeedLaWeed/proyecto-github.git
cd proyecto-github

3) se crearon index.html y readme.md con los siguientes comandos:
touch index.html
touch README.md

4) se hizo el first commit con los siguientes comandos:
git add index.html README.md
git commit -m "Primer commit: agregar index.html y README.md"

5) se modificó index.html agregando un h1

6) se hizo un commit "agregado titulo" con los siguientes comandos:
git add index.html
git commit -m "Agregado título"

7) se agregaron los pasos realizados a este README (abierto con VSC) 
y se hizo un commit con los siguientes comandos:
git add README.md
git commit -m "Actualizado el README.md con los pasos 1-6"

8) se hicieron los siguientes comandos:
git log
Se copió el hash del primer commit
touch log_com.txt
Se abrió log_com en VSC y se pegó el hash

9) se creó la rama estilos con los siguientes comandos:
git checkout -b estilos

10) se creó un styles.css con los siguientes comandos:
touch styles.css
Se abrió styles.css en VSC y se agregaron estilos para h1

11) se abrió index.html en VSC y se enlazó el css:
"<link rel="stylesheet" href="styles.css">"

12) se hizo el commit de agregar CSS con los siguientes comandos:
git add index.html styles.css
git commit -m "Agregado CSS"

13) se fusionaron las ramas estilos y main con los siguientes comandos:
git checkout main
git merge estilos

14) se anotaron los pasos 8-13 en este README. Se hizo commit:
git add README.md
git commit -m "Actualizado el README.md con los pasos 8-13"

15) se usó git reset:
git reset --soft HEAD~1
Se borró styles.css

16) se escribió en log_com abierto con VSC por qué se usó git reset

17) se volvió al primer commit con su hash, con los siguientes comandos:
git checkout ebca21702bc640a3475df866b9afea54449f339d

18) se volvió a la última versión con los siguientes comandos:
git checkout main

19) se anotaron los pasos restantes (14-20) a este README

20) se hizo el último commit y finalmente push a origin con los siguientes comandos:
git add README.md
git commit -m "Agregados los pasos restantes a README.md"
git push origin main