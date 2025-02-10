Práctica de Git y GitHub

Parte 1: Configuración Inicial
1. Configurar Git en tu equipo
Ejecuta los siguientes comandos en la terminal:
git config --global user.name Mario
git config --global user.email mariomompean9@gmail.com


2. Crear un nuevo repositorio en GitHub
Accede a GitHub.
Haz clic en "New Repository".
Asigna un nombre al repositorio y selecciona la opción "Initialize this repository with a README".




3. Clonar el repositorio en tu equipo
git clone https://github.com/mariomompean/practica-git.git
cd practica-git




Parte 2: Trabajo Individual con Git
1. Crear un archivo de prueba y hacer un commit
echo "# Proyecto Web" > index.html
git add index.html
git commit -m "Añadir archivo index.html"



2. Subir cambios al repositorio remoto
git push origin main

3. Actualizar el repositorio local con los cambios remotos
git pull origin main


Parte 3: Trabajo Colaborativo
1. Crear una nueva rama para una funcionalidad
git branch nueva-funcionalidad

git checkout nueva-funcionalidad

O también:
git checkout -b nueva-funcionalidad

2. Realizar cambios en la nueva rama y hacer commit
echo "<h1>Hola mundo</h1>" > index.html

git add index.html
git commit -m "Añadir título en index.html"

3. Subir la rama al repositorio remoto
git push origin nueva-funcionalidad

4. Realizar un Pull Request (PR) en GitHub
Un Pull Request (PR) es una solicitud para fusionar los cambios de una rama en otra. Para crear un PR:
Accede al repositorio en GitHub.
Ve a la pestaña "Pull Requests" y haz clic en "New Pull Request".
Selecciona la rama que contiene los cambios y compárala con main.

Revisa los cambios antes de enviarlos.
Escribe una descripción detallada del PR explicando los cambios realizados.
Haz clic en "Create Pull Request".

Espera revisiones y feedback de los compañeros o del profesor.
5. Revisar y fusionar cambios
Otro compañero revisa el PR y lo aprueba.

Si todo está correcto, se fusiona con la rama main.

Si hay sugerencias o cambios requeridos, deben realizarse antes de la aprobación.
Una vez aprobado, hacer clic en "Merge Pull Request" y eliminar la rama si ya no es necesaria.

6. Actualizar la rama local con los cambios aprobados
git checkout main
git pull origin main











Parte 4: Resolución de Conflictos
1. Generar un conflicto (de forma intencionada)
Dos alumnos editan la misma línea de index.html en diferentes ramas y hacen commits.
Alumno 1:




Alumno 2:







Ambos intentan fusionar sus ramas con main.
Primero fusionamos la del alumno 1.

Y ahora nos dará el conflicto.

2. Resolver el conflicto
Git avisará del conflicto.

Edita manualmente el archivo afectado, manteniendo los cambios correctos.

Una vez resuelto, ejecutar:
git add index.html
git commit -m "Resolver conflicto en index.html"
git push origin main


Parte 5: Entrega Final
Cada equipo debe entregar un repositorio con al menos:
Un README.md documentado.
Un historial de commits bien estructurado.
Uso de ramas y Pull Requests.
Al menos un conflicto resuelto correctamente.
Entrega
Enviar el enlace del repositorio a la plataforma de entrega.

Evaluación
Creación y clonación del repositorio: 20%
Uso correcto de commits y ramas: 30%
Trabajo colaborativo y Pull Requests: 30%
Resolución de conflictos y estructura del repositorio: 20%

