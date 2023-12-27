Ejercicio para comenzar a utilizar Git

-Desde el escritorio, he abierto una terminal de GitBash. He utilizado éstos 
comandos para moverme a la carpeta en la que voy a realizar el proyecto, crear una 
nueva, moverme a ella, crear un archivo README.md e inicializar el repositorio de 
Git.
    cd LEMON/ 
    mkdir Ejercicio-Git
    cd Ejercicio-Git/
    touch README.md

-En la página de GitHub, he creado un nuevo repositorio y he copiado la dirección 
que he introducido para conectar mi proyecto con mi nuevo repositorio y he 
comprobado si se ha establecido bien la conexión.
    git remote add origin git@github.com:xxxCoeNxxx/Ejercicio-Git.git
    git remote -v

-He creado un nuevo archivo por consola, he añadido todos los archivos al staging, 
he creado un commit y he subido los cambios a mi repositorio utilizando el flag -u 
para establecer la rama main como la predeterminada para los push.
    git add .
    git commit -m "Añadidos Archivo.md y README.md"
    git push -u origin main

-He añadido una nueva rama, cambiado a ella, he modificado mi Archivo.md por consola y el 
README.md, he hecho un nuevo commit y he subido los cambios.
    git checkout -b development
    echo "nuevo texto por consola" >> .\Archivo.md
    git add .
    git commit -m "Añadidos cambios y nueva rama"
    git push origin development