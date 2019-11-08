# TP_SO_I4_bondiola_
2 - Alfa clona el repositorio, crea una nueva rama, agrega sus datos y hace el push.

    git clone https://github.com/Barela-gabriela/TP_SO_I4_bondiola_
    git checkout -b Morel

(Agrega a datos.txt nombre y apellido, IP y hora)

    git add .
    git commit -m "Alfa modifica datos.txt"
    git push -u origin Morel

3 - Beta clona el repositorio, crea una nueva rama, agrega sus datos y hace el push.

    git clone https://github.com/Barela-gabriela/TP_SO_I4_bondiola_
    git checkout -b Passucci

(Agrega a datos.txt nombre y apellido, IP y hora)

    git add .
    git commit -m "Beta modifica datos.txt"
    git push -u origin Passucci

4 - Gamma intenta hacer el merge entre las ramas de Alfa y Beta en master pero se generan conflictos.

    git pull
    git merge origin/Morel
    git merge origin/Passucci

(Se generan conflictos y se procede a intentar corregirlos)

    git mergetool

(Se corrigen los conflictos modificando el datos.txt resultado en la interfaz)

    :wqa
    git add .
    git commit -m "Gamma hace merge desde ambas ramas"
    git push -u origin master

¿Se pueden mantener los dos datos? ¿Como?

Si, con la herramienta que proporciona el comando:

    git mergetool

(Lo que se hizo en el paso 4)

¿Se pueden mantener los dos datos sólo de un ALFA o BETA? ¿Como?

Se haria un (git merge rama_deseada) de los datos que se quieran tener en el master. Tambien podria ser (git checkout nombre_rama nombre_archivo)
