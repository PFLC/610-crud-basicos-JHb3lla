
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

Formularios para la elaboración de un CRUD

### 1. Crear (Create):

El formulario de creación permite a los usuarios agregar nuevos registros a la base de datos. Contendrá campos para ingresar la información necesaria para crear un nuevo elemento. Los campos generalmente estarán etiquetados y pueden incluir validaciones para garantizar que los datos ingresados sean correctos antes de enviarlos al servidor.

### 2. Leer (Read):

El formulario de lectura no es propiamente un formulario de entrada de datos, sino más bien una interfaz para mostrar los datos almacenados en la base de datos. Puede incluir opciones de búsqueda y filtrado para que los usuarios puedan encontrar rápidamente la información que están buscando. Esto podría ser una lista de elementos con la opción de ver detalles completos al hacer clic en un elemento específico.

### 3. Actualizar (Update):

El formulario de actualización permite a los usuarios modificar los datos de un registro existente en la base de datos. Al igual que el formulario de creación, contendrá campos etiquetados prellenados con la información actual del registro seleccionado. Los usuarios podrán realizar cambios en estos campos y luego enviar el formulario para actualizar los datos en la base de datos.

### 4. Eliminar (Delete):

El formulario de eliminación es un formulario simple que solicita confirmación antes de eliminar un registro de la base de datos. Por lo general, solo incluirá un mensaje de confirmación y un botón para confirmar la eliminación. Esto es importante para evitar eliminaciones accidentales de datos.

En resumen, un CRUD completo requerirá un conjunto de formularios que permitan a los usuarios realizar todas las operaciones básicas de creación, lectura, actualización y eliminación de datos en la base de datos. Cada formulario estará diseñado específicamente para su función, con campos y opciones relevantes para la operación que realiza.
