# Playtopia

Playtopia es una plataforma de juegos en línea donde puedes disfrutar de una variedad de juegos divertidos. Este archivo contiene el código fuente de la aplicación web de Playtopia.

## Estructura de archivos

- `app.py`: El archivo principal de la aplicación Flask que maneja las rutas y la lógica del servidor.
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
- `static/`: Directorio que contiene los archivos estáticos, como imágenes y hojas de estilo CSS.
- `helpers.py`: Módulo de ayuda que contiene funciones auxiliares utilizadas por `app.py`.
- `playtopia.db`: Base de datos SQLite que almacena la información de los usuarios.
- `gmNombreJuego.html`: Plantilla HTML de cada uno de los juegos.
- `gmNombreJuego.css`: Hoja de estilo de cada uno de los juegos.
- `gmNombreJuego.js`: Script de cada uno de los juegos.

## Requisitos

- Python 3.9 o superior
- Flask
- Flask-Session
- cs50

  ## Créditos > Integrantes

- Mabel Aryeris García Hernández
- Lesly Belén Vanegas Rayo
- Norman José Collado Bermúdez
