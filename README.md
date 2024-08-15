# Entrega_Final_RieraGalindoBustos
Entrega Final - Proyecto Coderhouse
# Proyecto Tienda de Libros

## Tablas

El proyecto cuenta con las siguientes tablas:

- **Usuarios:**
  - Se utilizan las tablas propias que vienen en Django para los usuarios.
  - Se agrega una tabla para incorporar los avatares de cada usuario.

- **Mi APP:**
  - **Libro:** Tabla que recopila la información de cada libro y su stock.
  - **Product image:** Permite asociar imágenes a cada libro.
  - **Order:** Permite hacer seguimiento de las órdenes cargadas.
  - **Order ítems:** Permite guardar cada ítem de cada orden.

## Pruebas y Funcionalidad

### Páginas Principales

Al entrar en la página sin loguearse, tendremos las siguientes solapas:

- **Barra de buscador:** Donde se podrán buscar productos. En caso de buscar productos existentes, nos traerá los mismos; en caso contrario, tendrá un mensaje que aclare que no se encontraron resultados con el dato solicitado.
- **Inicio:** Pantalla principal de nuestra página con un título ("Tienda de Libros, lo mejor para el lector") y, debajo de este, encontraremos algunas imágenes con frases de autores reconocidos.
- **About:** Una solapa donde encontraremos información acerca de los miembros del equipo y creadores del proyecto, junto con una breve descripción de nosotros.
- **Libros:** En esta solapa, podremos encontrar los productos cargados y, al hacer clic sobre los mismos, podremos ver más información acerca de ellos.
- **Cuenta:** Se habilitarán dos opciones: "Iniciar sesión" para usuarios ya registrados o "Crear Cuenta" para usuarios nuevos.
- **Pie de página:** Un mensaje de agradecimiento, el copyright con los apellidos de los miembros del equipo y el link a las redes sociales (las cuales están vinculadas a la página principal de cada red).

### Funcionalidades Adicionales

Si entramos logueados como un usuario normal, se agregan las siguientes solapas:

- **Crear pedido:** Donde se nos permitirá agregar los productos que queramos y la cantidad de los mismos que deseemos.
- **Consultar pedido:** Para poder ver todos los pedidos realizados (por el usuario que esté logueado en ese momento).
- **Cuenta:** Aparecerá con el avatar y nombre del usuario, reemplazando las opciones previamente vistas por:
  - **Ver cuenta:** Para consultar todos los datos registrados.
  - **Editar cuenta:** Para editar todos los campos (Username, Nombre, Apellido, Foto e incluso contraseña).
  - **Cerrar Sesión:** Para poder desloguearse del usuario.

Si entramos logueados como un usuario admin, se agrega la solapa:

- **Agregar libros:** Donde se nos permitirá agregar nuevos productos a los ya existentes, pudiendo cargar todos los datos correspondientes más imágenes.
- **Consultar pedido:** A diferencia del usuario normal, este podrá ver todos los pedidos cargados.

## Pasos para la Instalación del Proyecto

1. Descarga el repositorio con el comando `git clone <url>`.
2. Dirígete a la carpeta del proyecto usando `cd <nombre de la carpeta>`.
3. Crear / Activar el entorno virtual ejecutando `pipenv --python 3.12.4` (con la versión de Python que se tenga).
4. Ejecuta `pipenv shell` para iniciar el virtual environment.
5. Instala los requerimientos que se encuentran en el archivo `requirements.txt` con el comando `pipenv install -r requirements.txt`.
6. Ubícate dentro de la carpeta que contenga `manage.py`, en este caso, debes estar dentro de `proyectos_libros`.
7. Crear y ejecutar las migraciones:
   - Ejecuta el siguiente comando para preparar las migraciones de la base de datos: `python manage.py makemigrations`.
   - Ejecuta las migraciones para crear la base: `python manage.py migrate`.
8. Crea un usuario admin: `python manage.py createsuperuser`, completa los datos. Para este caso se usó el usuario `admin` y contraseña `admin`.
9. Ejecuta la aplicación en el servidor con `python manage.py runserver` para correr el servidor.

## Video del proyecto
 
**Link de Video:** [https://youtu.be/2SXZtheREOE?si=dVQ7yLu2EEOM3ydZ](https://youtu.be/2SXZtheREOE?si=dVQ7yLu2EEOM3ydZ)
