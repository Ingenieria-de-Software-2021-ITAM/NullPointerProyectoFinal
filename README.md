# NullPointerProyectoFinal
Integrantes:
Elisa Espinosa, Jorge Ortiz, Karen Arteaga y Victor Castillejos

ITAMPropone es una aplicación para proponer proyectos al ITAM en dónde les alumnes pueden votar por los mejores proyectos.
Las votaciones por los proyectos que a les estudiantes les interesan se manejan de la siguiente forma. En la pantalla de votaciones aparece una tabla con el nombre y la descripción de cada proyecto. Además, aparece la opción de votar por los proyectos que te gusten, pero solo permite votar una vez por cada uno. 

## 3. External Interface Requirements
  ### 3.1 Pantalla "Inicio de sesión"

![inicio de sesion](https://user-images.githubusercontent.com/47927104/143373730-0b9a6593-d1fe-4048-b5fb-f9e5bc387aeb.png)

###  3.2 Pantalla "Página principal" 

![página principal](https://user-images.githubusercontent.com/47927104/143373719-a88feed7-531b-4c80-868f-66b570197732.png)

###  3.3 Pantalla "Proponer proyecto" (Al presionar enviar, aparece un mensaje de proyecto enviado correctamente)

![proponer](https://user-images.githubusercontent.com/47927104/143380414-c894fe6c-6af0-453d-98cd-2f1a23b6a261.png)

###  3.4 Pantalla "Votar por proyectos" (Al votar por un proyecto, la opción de votar por ese proyecto desaparece)

![votar](https://user-images.githubusercontent.com/47927104/143373761-aa9f5906-07ce-49fe-a0d0-4f8b7e48d720.png)

###  3.5 Pantalla "Propuestas populares" (Aparecen las propuestas populares. Además, puedes buscar las propuestas por nombre, autor, descripción, etc)

![propuestas](https://user-images.githubusercontent.com/47927104/143373751-95bbf69a-ed9a-4a40-ba15-71c324c353ab.png)


## 4. Software Requirements
Poner 3 casos de uso por requirement

### 4.1 "Inicio de sesión"

#### &emsp; 4.1.1 Descripción y prioridad

 &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM tendrán permitido accesar a la página ITAMPropone. 

#### &emsp; 4.1.2 Secuencia de respuestas

 &emsp; Querer proponer un proyecto nuevo, poder ver votar por algún proyecto publicado. 

#### &emsp; 4.1.3 Requerimientos funcionales

- REQ-1: El usuario pueda escribir sus credenciales y sean autenticadas.
- REQ-2: De no ser autenticadas, mandar un mensaje de error.

### 4.2 "Publicar proyectos"

#### &emsp; 4.2.1 Descripción y prioridad

 &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM escriban y publiquen un posible proyecto. 

#### &emsp; 4.2.2 Secuencia de respuestas

 &emsp; Querer proponer una idea inovadora sobre que ayude a la comunidad itamita.

#### &emsp; 4.2.3 Requerimientos funcionales

- REQ-1: Poder escribir el nombre del proyecto
- REQ-2: Asignar automáticamente al autor del proyecto
- REQ-3: Escribir el contenido del proyecto
- REQ-4: Al presionar enviar, guardar toda la información (autor, nombre del proyecto y contenido) del nuevo proyecto en la base de datos.
- REQ-5: Agregar palabras clave sobre el contenido del texto (tema).
- REQ-6: No permitir enviar una propuesta con menos de 20 caracteres.

### 4.3 "Votar por proyectos"

#### &emsp; 4.3.1 Descripción y prioridad

 &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM observen y/o voten las propuestas de les otres miembres de la comunidad. 

#### &emsp; 4.3.2 Secuencia de respuestas

 &emsp; Votar por una propueta interesante. Observar las posibles propuestas que la comunidad está teniendo. Observar si alguna propuesta propia tiene popularidad. 

#### &emsp; 4.3.3 Requerimientos funcionales

- REQ-1: Poder buscar por autor, nombre del proyecto, tema o fecha de publicación. 
- REQ-2: Ver en una tabla las propuestas más populares antes de buscar.
- REQ-3: Poder observar en la tabla los proyectos que cumplan con la búsqueda de la tabla.
- REQ-4: Al votar por un proyecto, eliminar la opción de volver a votar, para evitar múltiples votos. 

### 4.4 "Eliminar proyectos"

#### &emsp; 4.4.1 Descripción y prioridad

 &emsp; Prioridad baja. Permitir que alguna propuesta sea eliminada por algún ejecutivo porque ya se cumplió y eliminar las propuestas menos populares después de cierto teimpo. 

#### &emsp; 4.4.2 Secuencia de respuestas

 &emsp; Alguna propuesta se volvió obsoleta porque ya se cumplió o no tiene popularidad. Liberar espacio en la base de datos. 

#### &emsp; 4.4.3 Requerimientos funcionales

- REQ-1: Revisar que las propuestas con la popularidad (menos del 10% de la comunidad) más baja tengan menos de 1 semestre de antigüedad. Las que no cumplan con este enunciado, serán eliminadas. 
- REQ-2: Poder eliminar alguna propuesta a voluntad.
- REQ-3: Eliminar todos los datos existentes sobre la propuesta. 

## Plan de Calidad
## Arquitectura
Elegimos una arquitectura por capas porque se enfoca en la distribución de roles y responsabilidades de forma jerárquica, además provee una forma muy efectiva de 
separación de responsabilidades.

Por ejemplo, una aplicación web típica está compuesta por una capa de presentación (funcionalidad relacionada con la interfaz de usuario), una capa de negocios (procesamiento de reglas de negocios) y una capa de datos (funcionalidad relacionada con el acceso a datos). Aplicaciones web Corporativas y sitios Web son ejemplos de esta arquitectura.
## Metodología

Implementamos la metodología AGILE porque utiliza periodos cortos de desarrollo llamado Sprints. Este enfoque permite hacer alteraciones para adaptarse conforme avanza el proyecto. 
## Código
https://app.moqups.com/mevbofgFeMiSIqXfxduif6CG89wNGW8F/view/page/af2dcae8a
## Documentación para replicar
## Propuesta económica
https://docs.google.com/spreadsheets/d/1X4sJLzmyVvuYx860ZdQr7GSJIlZPPlW4-zG5PzRE7gA/edit#gid=0
