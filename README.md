# Playtopia

Playtopia es una plataforma de juegos en línea donde puedes disfrutar de una variedad de juegos divertidos. Este archivo contiene el código fuente de la aplicación web de Playtopia.

## Estructura de archivos

- `layout.html`: La plantilla base de HTML que define la estructura común de todas las páginas.
- `index.html`: La plantilla HTML para la página de inicio que muestra los juegos disponibles.
- `login.html`: La plantilla HTML para la página de inicio de sesión.
- `register.html`: La plantilla HTML para la página para crear una cuenta.
- `ranking.html`: Este archivo representa la página de clasificación (ranking) del juego de la serpiente. Muestra una tabla con la posición, nombre de usuario y puntuación de los jugadores.
      - `extends "layout.html"`: Utiliza el archivo de diseño principal "layout.html" como plantilla base.
      - `block title`: Define el título de la página como "Ranking Serpiente".
      - `block main`: Contiene el contenido principal de la página, incluyendo el encabezado, la tabla y los datos de los jugadores.
      - `for loop in ranking`: Itera sobre los elementos de la variable "ranking" para mostrar la información de los jugadores en la tabla.
      - `if loop.index==1`: Aplica una clase CSS especial a la primera posición de la tabla.
      - `if loop.index == 1`: Muestra un ícono de corona en la primera posición de la tabla.
  
- `newPassword.html`: La plantilla HTML para la página de cambiar contraseña.

- `playtopia.db`: Base de datos SQLite que almacena la información de los usuarios.

###`static/`: Directorio que contiene los archivos estáticos, como imágenes y hojas de estilo CSS.
- En la carpeta `static` se encuentran los siguientes elementos relacionados con el proyecto:

- `img`: Carpeta que contiene las imágenes utilizadas en el proyecto.
- `sounds`: Carpeta que contiene los archivos de audio utilizados en el juego.
- `gmMemoria`: Carpeta que contiene los archivos CSS y JS específicos para el juego de memoria.
- `gmMemoria/images`: Carpeta que contiene las imágenes específicas para el juego de memoria.
- `script.js`: Archivo JavaScript principal que se utiliza en todo el proyecto.
- `style.css`: Hoja de estilo CSS principal que se aplica en todo el proyecto.
- Archivos JS y CSS específicos para cada juego: Estos archivos se encuentran dentro de carpetas con el nombre del juego correspondiente (por ejemplo, `gmJuego1.js` y `gmJuego1.css` para el primer juego, `gmJuego2.js` y `gmJuego2.css` para el segundo juego, y así sucesivamente).

- `gmNombreJuego.html`: Plantilla HTML de cada uno de los juegos.

  ### app.py
El archivo `app.py` es el archivo principal de la aplicación Flask. Contiene la configuración de la aplicación, las rutas y las funciones asociadas a cada una de ellas. Aquí se definen las siguientes rutas:

- `/`: Ruta principal que muestra el portafolio de juegos del usuario.
- `/login`: Ruta para iniciar sesión en la aplicación.
- `/logout`: Ruta para cerrar sesión.
- `/register`: Ruta para registrar nuevos usuarios.
- `/newPsw`: Ruta para cambiar la contraseña del usuario.
- `/gmCarrera`, `/gmMemory`, `/gmAdivinaPalabra`, `/gmAhorcado`, `/gmSpace`, `/gmSimon`, `/gmPPT`, `/gmSerpiente`, `/gmOperaciones`: Rutas correspondientes a cada juego individual. Algunas de estas rutas están actualmente comentadas y no contienen funcionalidad específica.
- `/ranking`: Ruta que muestra el ranking de los jugadores en el juego de la serpiente.

### helpers.py
El archivo `helpers.py` contiene funciones auxiliares utilizadas en la aplicación Flask. Incluye las siguientes funciones:

- `apology`: Función para mostrar un mensaje de disculpa al usuario en caso de error.
- `login_required`: Decorador que verifica si el usuario ha iniciado sesión antes de acceder a ciertas rutas.


## Requisitos

- Python 3.9 o superior
- Flask
- Flask-Session
- cs50

  ## Créditos > Integrantes

- Mabel Aryeris García Hernández
- Lesly Belén Vanegas Rayo
- Norman José Collado Bermúdez
