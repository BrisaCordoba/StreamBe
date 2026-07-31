# Sistema de Interpretación y Registro de Tiradas de Tarot

## 1. Problema 
Resuelve la falta de un registro organizado y digital para tiradas de Tarot, evitando que el usuario pierda la trazabilidad de sus lecturas o confunda las interpretaciones y relaciones entre cartas en lecturas pasadas.
Estudiantes y practicantes de Tarot que realizan lecturas periódicas (propias o para terceros) y necesitan documentar y analizar el histórico de tiradas de forma estructurada.
Permite consultar rápidamente lecturas pasadas, analizar patrones de cartas recurrentes y mantener una bitácora limpia y accesible sin depender de anotaciones en papel o chats dispersos.
 

## 2. Funcionalidades principales

1. Permitir el ingreso de una nueva lectura seleccionando las cartas del mazo, la posición/layout y la nota de interpretación.
2. Buscar lecturas registradas mediante palabras clave o por el nombre de una carta específica involucrada.
3. Filtrar el historial de lecturas según la persona receptora de la tirada o el tema abordado.
4. Actualizar o complementar las notas e interpretaciones de una lectura guardada previamente.
5. Borrar tiradas obsoletas o guardadas por error de la base de datos.
 

## 3. Datos principales a:

 **Título** Nombre o tema principal de la consulta.
 **Descripción:** Nombre de la persona a quien se le realiza la lectura.
 **Categoría** Clasificación según la temática abordada.
 **Fecha y hora:** Registro temporal de la sesión.
 **Cartas seleccionadas:** Lista de cartas involucradas y sus posiciones dentro del layout.
 **Notas de interpretación:** Texto detallado con el análisis y significado de la tirada. 
 **Marcador de Favorito:** Estado booleano para destacar tiradas relevantes.
 

## 4. SPEC

### Objetivo
Desarrollar una aplicación web sencilla y modular que funcione como bitácora digital para registrar, organizar, consultar y editar lecturas de Tarot de manera clara y estructurada.

### Usuario
Practicantes de Tarot que necesitan centralizar el historial de sus lecturas y mantener un seguimiento ordenado de sus interpretaciones.

### Funcionalidades
 Alta, edición, eliminación y visualización detallada de tiradas.
 Búsqueda por texto libre (cartas o títulos) y filtrado por categoría/consultante.
 Marcar tiradas favoritas para acceso rápido.

### Restricciones
 **Sin backend complejo ni servicios externos innecesarios:** Utilizar persistencia local para mantener una arquitectura simple en esta etapa.
 **Componentes enfocados:** Ningún archivo de componente debe superar las 200 líneas de código (principio de responsabilidad única).
 **Tipado estricto:** Prohibido el uso del tipo `any`. Todo debe estar explícitamente tipado.
 **Seguridad de código:** Queda prohibido eliminar archivos, instalar dependencias o alterar la estructura sin confirmación previa del usuario.

### Tecnología elegida
 **Lenguaje:** TypeScript (uso obligatorio).
 **Entorno / Framework:** React con componentes modulares.
 **Estilos:** CSS estándar o Tailwind CSS para una interfaz limpia y legible.
 
## 5. Prompt profesional: 

Actúa como un desarrollador senior y colabora en la construcción del MVP para una aplicación web de bitácora de tiradas de Tarot.

1. OBJETIVO Y TECNOLOGÍA:
Desarrolla una interfaz web modular utilizando TypeScript y React. El código debe ser limpio, altamente legible y seguir una arquitectura simple, evitando optimizaciones prematuras.

2. FUNCIONALIDADES A IMPLEMENTAR:
- Formulario para crear y editar tiradas de Tarot (campos: Título, Consultante, Fecha, Cartas seleccionadas, Notas de interpretación, Categoría, Favorito).
- Vista de lista y detalle para consultar tiradas guardadas.
- Sistema de búsqueda por palabra clave y filtrado por categoría/consultante.
- Opción de eliminar registros con confirmación del usuario.

3. REGLAS Y ESTILO DE CÓDIGO (AGENTS.MD):
- TypeScript obligatorio. No utilices el tipo 'any'; define interfaces explícitas para la entidad Tirada y sus dependencias.
- Principio de responsabilidad única: Cada componente debe ir en un archivo individual y no debe superar las 200 líneas de código.
- Limpieza: No dejes sentencias console.log ni código comentado en el resultado final.
- Nomenclatura: Usa camelCase en inglés para variables y funciones.

4. RESTRICCIONES DE ACTUACIÓN DEL AGENTE:
- Antes de escribir cualquier código, lee el contexto, realiza las preguntas aclaratorias necesarias y presenta un plan de trabajo paso a paso.
- No instales librerías adicionales ni modifiques el package.json sin solicitar autorización previa explícita.
- No elimines ni sobrescribas archivos existentes sin confirmación.


## Challenge de validación

voy a revisar estos puntos para estar segura de que todo quedó bien:

1. **¿Funciona todo bien?**
   Probar si deja crear una tirada nueva sin errores.
   Probar si deja editar los datos de una lectura ya guardada.
   Probar si el botón de eliminar borra la tirada correcta.
   Probar que el buscador y los filtros funcionen bien.

2. **¿Respeta las reglas de código?**
   Revisar que no haya usado any en ningún lado.
   Confirmar que no hayan quedado console.log sueltos.
   Verificar que ningún archivo tenga más de 200 líneas.

3. **¿La estructura está ordenada?**
   Ver que cada componente esté en su propio archivo.
   Que los nombres de las carpetas y archivos sean claros y estén en inglés (camelCase).

4. **¿Los datos se guardan bien?**
   Guardar una tirada, recargar la página y revisar que la información siga ahí y no se haya borrado.

5. **¿La pantalla es clara?**
   Que la lista de tiradas se vea prolija.
   Que las cartas, las fechas y las notas de la lectura se entiendan fácil a primera vista.

6. **¿Siguió los límites antes de programar?**
   Verificar que me haya explicado su plan antes de escribir el código.
   Confirmar que no haya instalado librerías raras ni borrado archivos sin preguntar primero.
