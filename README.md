
# Aplicación CRUD de PHP

Este repositorio contiene una aplicación PHP CRUD (Create, Read, Update, Delete) simple. Es una demostración básica de cómo integrar PHP con una base de datos MySQL para gestionar datos de usuarios. La aplicación permite a los usuarios agregar, ver, editar y eliminar información de usuario.

## Tecnologías Utilizadas

- **PHP:** Lenguaje de script del lado del servidor utilizado para el desarrollo web.
- **MySQL:** Sistema de gestión de base de datos utilizado para almacenar datos de usuario.
- **HTML & CSS:** Utilizados para estructurar y dar estilo a las páginas web.
- **Tailwind CSS:** Un framework de CSS utilitario para el desarrollo rápido de interfaces de usuario.

## Páginas y Funcionalidades

### 1. Página de Inicio (`display.php`)

![Página de Inicio](images/display.png)

- **Funcionalidad:** Muestra todos los usuarios de la base de datos en un formato de tabla.
- **Características:** 
  - Ver todos los usuarios.
  - Enlaces de navegación para agregar, editar o eliminar información de usuario.

### 2. Agregar Usuario (`user.php`)

![Agregar Usuario](images/add.png)

- **Funcionalidad:** Permite agregar un nuevo usuario a la base de datos.
- **Características:** 
  - Formulario para ingresar detalles del usuario (nombre, correo electrónico, teléfono móvil, contraseña).
  - Validación de datos y envío a la base de datos.

### 3. Editar Usuario (`edit.php`)

![Editar Usuario](images/edit.png)

- **Funcionalidad:** Permite editar detalles de usuarios existentes.
- **Características:** 
  - Formulario prellenado con la información actual del usuario.
  - Actualización de detalles del usuario en la base de datos.

### 4. Eliminar Usuario (`delete.php`)

- **Funcionalidad:** Facilita la eliminación de un usuario de la base de datos.
- **Características:** 
  - Eliminación de información de usuario basada en el ID de usuario.

## Conexión a la Base de Datos (`connect.php`)

- **Propósito:** Establece una conexión con la base de datos MySQL.
- **Credenciales:** Utiliza nombre de host, nombre de usuario, contraseña y nombre de la base de datos para la conexión.

## Cómo Ejecutar

1. Clona el repositorio en tu máquina local.
2. Configura un entorno PHP y MySQL (como XAMPP).
3. Crea la base de datos usando phpmyadmin.
4. Ejecuta la aplicación en un servidor local.

## Nota de Seguridad

Esta aplicación es una demostración básica y no implementa medidas avanzadas de seguridad. Es recomendable utilizar declaraciones preparadas (prepared statements) u ORM para las interacciones con la base de datos para prevenir ataques de inyección SQL.

---

Siéntete libre de contribuir a este proyecto o sugerir mejoras. Para cualquier consulta o problema, por favor abre un issue en este repositorio.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------
INVESTIGACION

Formularios para la elaboracion de un CRUD
Un CRUD (Crear, Leer, Actualizar y Eliminar) es una funcionalidad básica en muchas aplicaciones de software que permite la gestión de datos. Aquí te muestro un ejemplo básico de cómo podrían ser los formularios para cada una de las operaciones CRUD:

1. Crear (Create)
Formulario de Creación 
<form action="crear.php" method="POST">
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre" required>
    <label for="edad">Edad:</label>
    <input type="number" id="edad" name="edad" required>
    <button type="submit">Crear</button>
</form>

2. Leer (Read)
Formulario de Búsqueda: 
<form action="buscar.php" method="GET">
    <label for="buscar">Buscar:</label>
    <input type="text" id="buscar" name="buscar">
    <button type="submit">Buscar</button>
</form>

3. Actualizar (Update)
Formulario de Edición: 
<form action="actualizar.php" method="POST">
    <input type="hidden" id="id" name="id" value="ID_DEL_REGISTRO_A_ACTUALIZAR">
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre" required>
    <label for="edad">Edad:</label>
    <input type="number" id="edad" name="edad" required>
    <button type="submit">Actualizar</button>
</form>

4. Eliminar (Delete)
Formulario de Eliminación: 
<form action="eliminar.php" method="POST">
    <input type="hidden" id="id" name="id" value="ID_DEL_REGISTRO_A_ELIMINAR">
    <p>¿Estás seguro de que quieres eliminar este registro?</p>
    <button type="submit">Eliminar</button>
</form>

Recuerda que estos son solo ejemplos básicos y que la implementación real puede variar dependiendo del lenguaje de programación y del sistema de gestión de base de datos que estés utilizando. Además, asegúrate siempre de validar y sanear los datos recibidos del usuario para prevenir ataques de seguridad como inyección de SQL.

