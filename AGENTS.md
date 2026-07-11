# AGENTS.md

## Proyecto
Sistema de Gestión para la Biblioteca  
Es una aplicación para controlar el inventario de libros de la escuela, registrar a los alumnos y manejar el sistema de préstamos y devoluciones para que no se pierda nada

## Comandos Principales
-npm run start  - Para levantar el entorno y probar la app.
-npm run lint - Para chequear que no haya errores de sintaxis o cosas raras en el código.

## Estilo de Código
-Idioma - Las tablas de la base de datos, las variables y las funciones van todas en español. Los comentarios que expliquen lógica compleja van en inglés.
-Base de Datos - El diseño de las tablas tiene que cumplir con la Tercera Forma Normal (3FN). Todo lo que sea palabras clave de SQL (como SELECT, INSERT, WHERE, JOIN) se escribe en mayúsculas.
-Variables - Usar nombres claros y descriptivos en minúsculas, separados por guiones bajos (por ejemplo: `id_alumno`, `fecha_prestamo`). Nada de nombres genéricos como `x` o `dato`.

## Comportamiento del Agente

### Qué podés hacer directamente 
-Armar las consultas SQL para buscar libros por título, autor o categoría.
-Programar las funciones lógicas que calculen si un préstamo está vencido o si hay stock.
-Agregar comentarios claros en el código donde falte documentación.

### Qué NO tenés que hacer sin preguntarme antes 
-Tocar o cambiar las claves primarias (PK) o foráneas (FK) de las tablas que ya definí.
-Hacer bajas físicas en la base de datos (siempre usar bajas lógicas con un estado).
-Instalar librerías o dependencias nuevas con npm sin avisar.
-Cambiarme el orden o la estructura de las carpetas del proyecto.
