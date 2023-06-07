# Instalación de Moodle-Equipo4

## Moodle y dependencias
- Instalación con docker-compose 

## Usuarios y Contraseñas que se deben cambiar en el archivo docker-compose.yml
- MARIADB_USER=bn_moodle
- MARIADB_PASSWORD=bitnami

### Correr localmente usando docker

1. Clonar el repositorio al directorio local de instalación donde trabajemos nuestro docker
git clone https://github.com/Ace28w/Moodle-Equipo4.git

2. Para correr los contenedores

cd Moodle-Equipo4

- Consideración a tomar

--> Si no esta instalado el docker compose lo puedes descargar e instalar con el siguiente comando:

sudo apt  install docker-compose

--> Como recomendación apagar contenedores docker que estén en ejecución con:

docker stop "ID"

- Ahora con el siguiente comando lo podemos levantar

docker-compose up

- Para saber que ya esté en funcionamiento deberá aparecer el FOREGROUND, como vemos en la imagen de abajo

![Moodle-Screen09](Img/Fore.png)


3. Para detener los contenedores

$docker-compose stop

# Paso 1) Correr Moodle

- http://TuIP:80/ --> Cambiamos la IP por la nuestra
- Usuario: user
- Password: bitnami

# Paso 2) Entrar en nuestro Moodle

- Accediendo a nuestro moodle desde nuestra IP nos vamos a log in

![Moodle-Screen01](Img/Inicio.png)

- Ya dentro podemos nuestras credenciales para entrar en modo administrador que se menciona en el paso 1

![Moodle-Screen02](Img/Login.png)

- Ahora vemos que hemos iniciado en modo administrador a nuestro moodle

![Moodle-Screen03](Img/Dentro.png)

# Paso3) Creación de un curso

- Como primer paso habilitamos el modo edición y nos vamos en my courses
- En los 3 puntos estará para agregar un nuevo curso

![Moodle-Screen04](Img/Cursos.png)

- Entonces llenamos los datos necesarios como el nombre que queramos

![Moodle-Screen05](Img/Agregarcurso.png)

- Bajamos hasta el final y vemos que esta confirmar, le damos click

![Moodle-Screen06](Img/ConfirmarCurso.png)

- Ahora vemos que estaos dentro del curso y podremos agregar las actividades entre varias cosas

![Moodle-Screen07](Img/DentroCurso.png)

- Ahora si nos vamos en my courses podemos ver que se encuentra el que teníamos y el nuevo, donde acá aparecen todos nuestros cursos creados

![Moodle-Screen08](Img/CursoFinal.png)
