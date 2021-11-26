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
  - Iniciar sesión: el usuario inicia sesión con el correo institucional o con su cuneta de administrador.
  - Página principal: el usuario elige una de las tres opciones de funcionalidades (proponer un proyecto, votar por proyectos, consultar proyectos seleccionados)
  - Página principal (versión administrador): se muestra la opción de ver preoyectos y cerrar sesión.
  - Proponer un proyecto: el usuario envía una propuesta de proyecto.
  - Votar: el usuario vota por los proyectos que más le agraden.
  - Consultar proyectos: se exhiben los proyectos con más votos hasta el momento.
  - Ver proyectos: el administrador maneja los proyectos existentes.

  Página principal:
  - Proponer un proyecto: manda al usuario a la pantalla "Proponer un proyecto".
  - Votar: manda al usuario a la pantalla "Votar".
  - Consultar un proyecto: manda al usuario a la pantalla "Consultar un proyecto".
  - Cerrar Sesión: se cierra la sesión actual.

  Página principal (versión administrador):
  - Ver proyectos: manda al administrador a la pantalla "Ver proyectos".
  - Cerrar sesión: se cierra la sesión actual.
  
  Iniciar sesión:
  - Correo: el usuario ingresa su correo institucional o con su cuenta de administrador.
  - Contraseña: el usuario ingresa su contraseña.
  - Ingresar: comprueba que los datos ingresados por el usuario sean correctos y lo manda a la página principal.
  
  Proponer un proyecto:
  - Nombre del Proyecto: el usuario ingresa el nombre del proyecto que quiere compartir con la comunidad.
  - Autores: el usuario escribe el nombre de los autores del proyecto.
  - Descripción: el usuario da una descripción detallada del proyecto que quiere proponer.
  - Imagen: el usuario asigna una imagen a la propuesta del proyecto.
  - Enviar: comprueba que los datos ingresados por el usuario sean correctos y que el proyecto no exista en la base de datos.
  - Página principal: regresa a la vista de la página principal.
  
  Votar:
  - Barra de búsqueda: el usuario escribe los datos del proyecto que desea buscar.
  - Botón con ícono de corazón: genera un voto por el proyecto que se muestra en pantalla y avanza al siguiente proyecto.
  - Botón con ícono de cruz: avanza al siguiente proyecto.
  - Botón flecha: regresa al proyecto anterior.
  - 
  - Página principal: regresa a la vista de la página principal.

  Consultar proyectos:
  - Barra de búsqueda: el usuario escribe los datos del proyecto que desea buscar.
  - Buscar: se muestran los proyectos que resultan de la búsqueda.
  - Página principal: regresa a la vista de la página principal.

  Ver proyectos:
  - Barra de búsqueda: el usuario escribe los datos del proyecto que desea buscar.
  - Buscar: se muestran los proyectos que resultan de la búsqueda.
  - Eliminar: muestra una ventana "pop-up" para verificar si la selección fue correcta.
  - Aceptar: elimina el proyecto seleccionado.
  - Cancelar: cancela la acción.
  - Página principal: regresa a la vista de la página principal versión administrador.

  ### 2.3 Clases de usuario y características
  
  Usuarios generales, estudiantes, exalumnes y profesores del ITAM que buscan participar en la selección de proyectos de la comunidad ITAM, ya sea a través de propuestas de proyectos, del voto o de la consulta.
  
  Usuarios administradores, integrantes de la comunidad ITAM que tienen permiso de manejar los proyectos propuestos. 
  
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
  
  ITAMPropone está desarrollado en el ambiente de prototipado https://moqups.com, por lo que requiere de una conexión estable de internet, así como el enlace para visualizar el prototipo del sistema.

## 3. Requerimientos de interfaz externa
  ### 3.1 Vista "Inicio de sesión"

![inicio de sesion](https://user-images.githubusercontent.com/47927104/143373730-0b9a6593-d1fe-4048-b5fb-f9e5bc387aeb.png)

###  3.2 Vista "Página principal" 

![página principal](https://user-images.githubusercontent.com/47927104/143512608-333011ae-c7df-4ba3-a37b-81cfcda3fc09.png)

###  3.3 Vista "Página principal (versión administrador)"

![página principal-admin](https://user-images.githubusercontent.com/47927104/143512610-7d9dbf24-cc9a-402f-8b45-ca35e8a03bb8.png)

###  3.4 Vista "Proponer proyecto" (Al presionar enviar, aparece un mensaje de proyecto enviado correctamente)

![proponer](https://user-images.githubusercontent.com/47927104/143509497-3efa3db2-0c4d-45ea-a09c-3fd0edd5d284.png)

###  3.5 Vista "Votar por proyectos" (Al votar por un proyecto, aparece otro proyecto)

![votar](https://user-images.githubusercontent.com/47927104/143510044-e73c8b71-2370-42cb-92d7-76fac376edfb.png)
![votar2](https://user-images.githubusercontent.com/47927104/143510048-a0e9241b-1354-46d9-a3c7-023b49cef448.png)

###  3.6 Vista "Propuestas populares" (Aparecen las propuestas populares. Además, puedes buscar las propuestas por nombre, autor, descripción, etc)

![propuestas](https://user-images.githubusercontent.com/47927104/143509731-11628dc9-951f-4a60-89e8-f2eee5531ab0.png)

###  3.7 Pantalla "Eliminar proyectos" 

![verproyectos](https://user-images.githubusercontent.com/47927104/143512611-03069dc9-b83b-4fd6-8915-6b39d7d63fe9.png)

## 4. Requerimientos de software

### 4.1 Inicio de sesión

#### &emsp; 4.1.1 Descripción y prioridad

 &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM tengan permitido accesar a la página ITAMPropone. Permitir que los administradores tengan acceso permitido a ITAMPropone en su versión de administrador.

#### &emsp; 4.1.2 Secuencia de respuestas

 &emsp; Para los usuarios generals, querer proponer un proyecto nuevo, poder ver votar por algún proyecto publicado, consultar la popularidad de los proyectos existentes. Para los administradores, poder manejar los proyectos existentes.

#### &emsp; 4.1.3 Requerimientos funcionales

- REQ-1: El usuario pueda escribir sus credenciales y sean autenticadas.
- REQ-2: De no ser autenticadas, mandar un mensaje de error.
- REQ-3: Redirigir al usuario a la versión general o administrador según los permisos que tenga.

### 4.2 Publicar proyectos

#### &emsp; 4.2.1 Descripción y prioridad

 &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM escriban y publiquen un posible proyecto. 

#### &emsp; 4.2.2 Secuencia de respuestas

 &emsp; Querer proponer una idea innovadora que ayude a la comunidad itamita.

#### &emsp; 4.2.3 Requerimientos funcionales

- REQ-1: Poder escribir el nombre del proyecto.
- REQ-2: Asignar automáticamente al autor del proyecto.
- REQ-3: Escribir el contenido del proyecto.
- REQ-4: Al presionar enviar, guardar toda la información (autor, nombre del proyecto y contenido) del nuevo proyecto en la base de datos.
- REQ-5: Agregar palabras clave sobre el contenido del texto (tema).
- REQ-6: No permitir enviar una propuesta con menos de 20 caracteres.
- REQ-7: Añadir imágenes.

### 4.3 Votar por proyectos

#### &emsp; 4.3.1 Descripción y prioridad

 &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM observen y/o voten las propuestas de les otres miembres de la comunidad. 

#### &emsp; 4.3.2 Secuencia de respuestas

 &emsp; Votar por una propueta interesante. Observar las posibles propuestas que la comunidad está teniendo. Observar si alguna propuesta propia tiene popularidad. 

#### &emsp; 4.3.3 Requerimientos funcionales

- REQ-1: Al votar por un proyecto, eliminar la opción de volver a votar, para evitar múltiples votos.
- REQ-2: Si no votas por el proyecto, no debe aparecer de nuevo en feed de votaciones. A menos que el usuario decida regresar al proyecto anterior.
- REQ-3: Poder leer las descripciones de los proyectos y ver las imágenes. 
- REQ-4: Poder darle un valor especial a ese proyecto, en caso de que le encante al usuario. 

### 4.4 Eliminar proyectos

#### &emsp; 4.4.1 Descripción y prioridad

 &emsp; Prioridad baja. Permitir que alguna propuesta sea eliminada por algún ejecutivo porque ya se cumplió y eliminar las propuestas menos populares después de cierto tiempo. 

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
