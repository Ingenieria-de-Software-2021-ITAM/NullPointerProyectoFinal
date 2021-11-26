# NullPointerProyectoFinal
Integrantes:
Elisa Espinosa, Jorge Ortiz, Karen Arteaga y Victor Castillejos

ITAMPropone es una aplicación para proponer proyectos al ITAM en dónde les alumnes pueden votar por los mejores proyectos.
Las votaciones por los proyectos que a les estudiantes les interesan se manejan de la siguiente forma. En la pantalla de votaciones aparece una tabla con el nombre y la descripción de cada proyecto. Además, aparece la opción de votar por los proyectos que te gusten, pero solo permite votar una vez por cada uno. 

## 1. Introducción
  ### 1.1 Objetivo
  
  El objetivo de este documento es presentar una descripción detallada del software ITAMPropone. Se explicarán los requerimientos y funcionalidades del software, así como las interfaces, el alcance y las restricciones que presenta el sistema en su versión actual.
  
  ### 1.2 Convenciones del documento
  
  Este documento se creó con base en el modelo IEEE para especificación de requerimientos de software (Software Requirements Specification)
  
  ### 1.3 Sugerencias de lectura
  
  Este documento está escrito para estudiantes y profesores del departamento de Ingeniería en Computación del Instituto Tecnológico Autónomo de México que quieran conocer sobre los proyectos desarrollados en el curso de Ingeniería de Software.
  
  ### 1.4 Extensión del producto
  
  ITAMPropone es un proyecto en fase de prototipo que está dirigido específicamente para la clase Ingeniería de Software del Instituto Tecnológico Autónomo de México. El objetivo de ITAMPropone es que los integrantes de la comunidad ITAM tengan un ambiente web seguro y confiable en el que puedan proponer y votar por los proyectos que se desarrollan dentro del campus.
  
  ### 1.5 Referencias
  ITAMPropone prototipo (versión actual): https://app.moqups.com/mevbofgFeMiSIqXfxduif6CG89wNGW8F/view/page/af2dcae8a

  Repositorio en GitHub: https://github.com/Ingenieria-de-Software-2021-ITAM/NullPointer-Markdown

  IEEE template for Software Requirement Specification: https://goo.gl/nsUFwy

## 2. Descripción general

  ### 2.1 Perspectiva del producto
  
  ITAMPropone se desarrolló para los integrantes de la comunidad ITAM. Es una página web en la que los estudiantes pueden proponer proyectos a la comunidad ITAM, votar por las mejores ideas y consultar el ranking de los proyectos con más votos. 
ITAMPropone se desarrolló para ser reproducido en internet como página web.

  ### 2.2 Funciones del producto
  
  Vistas:
  - Iniciar sesión: el usuario inicia sesión con el correo institucional.
  - Página principal: el usuario elige una de las tres opciones de funcionalidades (proponer un proyecto, votar por proyectos, consultar proyectos seleccionados)
  - Proponer un proyecto: el usuario envía una propuesta de proyecto.
  - Votar por proyectos: el usuario vota por los proyectos que más le agraden.
  - Proyectos seleccionados: se exhiben los proyectos con más votos hasta el momento.
  
  Iniciar sesión:
  - Correo: el usuario ingresa su correo institucional.
  - Contraseña: el usuario ingresa su contraseña.
  - Ingresar: comprueba que los datos ingresados por el usuario sean correctos.
  
  Proponer un proyecto:
  - Nombre del Proyecto: el usuario ingresa el nombre del proyecto que quiere compartir con la comunidad.
  - Autores: el usuario escribe el nombre de los autores del proyecto.
  - Descripción: el usuario da una descripción detallada del proyecto que quiere proponer.
  - Enviar: comprueba que los datos ingresados por el usuario sean correctos y que el proyecto no exista en la base de datos.
  - Página principal: regresa a la vista de la página principal.
  
  Votar por proyectos:
  - Barra de búsqueda: el usuario escribe los datos del proyecto que desea buscar.
  - Buscar: se muestran los proyectos que resultan de la búsqueda.
  - Votar: genera un voto por el proyecto que se muestra en pantalla.
  - Página principal: regresa a la vista de la página principal.

  Consultar proyectos:
  - Barra de búsqueda: el usuario escribe los datos del proyecto que desea buscar.
  - Buscar: se muestran los proyectos que resultan de la búsqueda.
  - Página principal: regresa a la vista de la página principal.

  ### 2.3 Clases de usuario y características
  
  Usuarios generales, estudiantes del ITAM que buscan participar en la selección de proyectos de la comunidad ITAM, ya sea a través de propuestas de proyectos, del voto o de la consulta.
  
  ### 2.4 Ambiente de operación
  
  Internet 
  
  ### 2.5 Restricciones de diseño e implementación
  
  ITAMPropone está desarrollado como prototipo en el ambiente de desarrollo https://moqups.com. Tanto el diseño como la implementación están en la fase de prototipo y dependen en su totalidad del sistema en el que se están desarrollando. 
  
  ### 2.6 Documentación de usuario
  
  La guía para la visualización del prototipo del sistema ITAMPropone es la siguiente.
  1. Verificar que se cuenta con una conexión de internet estable.
  2. Ingresar a https://app.moqups.com/mevbofgFeMiSIqXfxduif6CG89wNGW8F/view/page/ad64222d5#
  3. Navegar por el prototipo con los botones que aparecen en pantalla. 

  El documento de replicación del sistema se encuentra en: 
  
  ### 2.7 Suposiciones y dependencias
  
  ITAMPropone está desarrollado en el ambiente de prototipación https://moqups.com, por lo que requiere de una conexión estable de internet, así como el enlace para visualizar el prototipo del sistema.

## 3. External Interface Requirements
  ### 3.1 Pantalla "Inicio de sesión"

![inicio de sesion](https://user-images.githubusercontent.com/47927104/143373730-0b9a6593-d1fe-4048-b5fb-f9e5bc387aeb.png)

###  3.2 Pantalla "Página principal" 

![página principal](https://user-images.githubusercontent.com/47927104/143373719-a88feed7-531b-4c80-868f-66b570197732.png)

###  3.3 Pantalla "Proponer proyecto" (Al presionar enviar, aparece un mensaje de proyecto enviado correctamente)

![proponer](https://user-images.githubusercontent.com/47927104/143509497-3efa3db2-0c4d-45ea-a09c-3fd0edd5d284.png)


###  3.4 Pantalla "Votar por proyectos" (Al votar por un proyecto, la opción de votar por ese proyecto desaparece)

![votar](https://user-images.githubusercontent.com/47927104/143381921-3313d73a-eb63-46ec-88d2-e3feb7b68ff3.png)

###  3.5 Pantalla "Propuestas populares" (Aparecen las propuestas populares. Además, puedes buscar las propuestas por nombre, autor, descripción, etc)

![propuestas](https://user-images.githubusercontent.com/47927104/143509731-11628dc9-951f-4a60-89e8-f2eee5531ab0.png)


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
- REQ-7: Añadir fotos

### 4.3 "Votar por proyectos"

#### &emsp; 4.3.1 Descripción y prioridad

 &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM observen y/o voten las propuestas de les otres miembres de la comunidad. 

#### &emsp; 4.3.2 Secuencia de respuestas

 &emsp; Votar por una propueta interesante. Observar las posibles propuestas que la comunidad está teniendo. Observar si alguna propuesta propia tiene popularidad. 

#### &emsp; 4.3.3 Requerimientos funcionales

- REQ-1: Al votar por un proyecto, eliminar la opción de volver a votar, para evitar múltiples votos.
- REQ-2: Si no votas por el proyecto, no debe aparecer de nuevo en feed de votaciones.
- REQ-3: Poder leer las descripciones de los proyectos y ver las imágenes. 

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
