# Especificación de requerimientos de software para ITAMPropone
--- 
Autores:
- Arteaga Mendoza Karen
- Castillejos Victor
- Espinosa Elisa
- Ortiz Jorge
---
--- 
Versión 1.0
--- 
Noviembre 2021
---
## Tabla de contenidos
  1. [Introducción](#introduccion)
  2. [Descripción general](#descripcion-general)
  3. [Requerimientos de interfaz externa](#requerimientos1)
  4. [Funcionalidades del sistema](#requerimientos2)
  5. [Otros requerimientos](#otros-requerimientos)

## 1. Introducción <a name="introduccion"></a>
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

## 2. Descripción general <a name="descripcion-general"></a>

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

  En su versión actual de prototipo, el ambiente de operación de ITAMPropone está sujeto al ambiente de operación de la página web https://moqups.com.
  
  ### 2.5 Restricciones de diseño e implementación
  
  ITAMPropone está desarrollado como prototipo en el ambiente de desarrollo https://moqups.com. Tanto el diseño como la implementación están en la fase de prototipo y dependen en su totalidad del sistema en el que se están desarrollando. 
  
  ### 2.6 Documentación de usuario

  El documento de replicación del sistema se encuentra en: https://github.com/Ingenieria-de-Software-2021-ITAM/NullPointerProyectoFinal/blob/main/ProyectoFinalNullPointer.md#documentación-para-replicar
  
  ### 2.7 Suposiciones y dependencias
  
  ITAMPropone está desarrollado en el ambiente de prototipado https://moqups.com, por lo que requiere de una conexión estable de internet, así como el enlace para visualizar el prototipo del sistema.

## 3. Requerimientos de interfaz externa <a name="requerimientos1"></a>

  ### 3.1 Interfaces de Usuario
  
   #### 3.1.1 Vista "Inicio de sesión"

   ![inicio de sesion](https://user-images.githubusercontent.com/47927104/143373730-0b9a6593-d1fe-4048-b5fb-f9e5bc387aeb.png)

   ####  3.1.2 Vista "Página principal" 

   ![página principal](https://user-images.githubusercontent.com/47927104/143512608-333011ae-c7df-4ba3-a37b-81cfcda3fc09.png)

  ####  3.1.3 Vista "Página principal (versión administrador)"

  ![página principal-admin](https://user-images.githubusercontent.com/47927104/143512610-7d9dbf24-cc9a-402f-8b45-ca35e8a03bb8.png)

  ####  3.1.4 Vista "Proponer proyecto" (Al presionar enviar, aparece un mensaje de proyecto enviado correctamente)

  ![proponer](https://user-images.githubusercontent.com/47927104/143509497-3efa3db2-0c4d-45ea-a09c-3fd0edd5d284.png)

  #### 3.1.5 Vista "Votar por proyectos" (Al votar por un proyecto, aparece otro proyecto)

  ![votar](https://user-images.githubusercontent.com/47927104/143510044-e73c8b71-2370-42cb-92d7-76fac376edfb.png)
  ![votar2](https://user-images.githubusercontent.com/47927104/143510048-a0e9241b-1354-46d9-a3c7-023b49cef448.png)

  ####  3.1.6 Vista "Propuestas populares" (Aparecen las propuestas populares. Además, puedes buscar las propuestas por nombre, autor, descripción, etc)

  ![propuestas](https://user-images.githubusercontent.com/47927104/143509731-11628dc9-951f-4a60-89e8-f2eee5531ab0.png)

  ####  3.1.7 Pantalla "Eliminar proyectos" 

  ![verproyectos](https://user-images.githubusercontent.com/47927104/143512611-03069dc9-b83b-4fd6-8915-6b39d7d63fe9.png)

  ### 3.2 Interfaces de hardware
  
  ITAMPropone en su versión actual es accesible a cualquier integrante de la comunidad ITAM que posea el enlace de visualización y un navegador web en cualquier dispositivo que soporte la herramienta de desarrollo https://moqups.com hasta la fecha.
  ITAMPropone, en su versión final, será accesible a la comunidad ITAM a través de cualquier dispositivo que cuente con un navegador de internet.
  - Computadora de escritorio
  - Computadora personal
  - Smartphone
  - Tablet 
  - Otros dispositivos con acceso al navegador
  
  ### 3.3 Interfaces de software
  
  ITAMPropone en su versión actual es accesible a cualquier integrante de la comunidad ITAM que posea el enlace de visualización y un navegador web soporte la herramienta de desarrollo https://moqups.com hasta la fecha.
  ITAMPropone, en su versión final, será accesible a la comunidad ITAM a través de un navegador web.

## 4. Funcionalidades del sistema <a name="requerimientos2"></a>

  ### 4.1 Inicio de sesión

   #### &emsp; 4.1.1 Descripción y prioridad

   &emsp; Prioridad alta. Permitir que les alumnes, exalumnes y profesores del ITAM tengan permitido accesar a la página ITAMPropone. Permitir que los administradores tengan acceso permitido a ITAMPropone en su versión de administrador.    

   #### &emsp; 4.1.2 Secuencia de respuestas

  &emsp; Para los usuarios generals, querer proponer un proyecto nuevo, poder ver votar por algún proyecto publicado, consultar la popularidad de los proyectos existentes. Para los administradores, poder manejar los proyectos existentes.
  
  #### &emsp; Caso de uso
  

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

## 5. Otros requerimientos <a name="otros-requerimientos"></a>

  ### 5.1 Requerimientos de desempeño
  
  ITAMPropone requiere de un equipo con conexión estable a internet que soporte la herramienta de prototipado https://moqups.com, así como el enlace para visualizar la versión actual (https://app.moqups.com/mevbofgFeMiSIqXfxduif6CG89wNGW8F/view/page/af2dcae8a)
  
  ### 5.2 Requerimientos de seguridad
  
  Para asegurar que ninguno de los usuarios que visualizan el prototipo de ITAMPropone los desarrolladores sugieren a los usuarios conectarse a una red segura y leer los términos y condiciones del entorno de desarrollo https://moqups.com en el que se manejó el sistema. Además, en su versión final, ITAMPropone deberá seguir las pautas de seguirdad de software.   
  - Autenticación: ITAMPropone implementará la verificación en dos pasos con el correo institucional para validad la identidad de sus usuarios.
  - Autorización: solo los usuarios con cuenta de administrador podrán realizar las acciones permitidas para los administradores. Las cuentas de usuarios generales tendrán acceso limitado al manejo de los proyectos.
  - Confidencialidad: como ITAMPropone maneja información sensible del usuario, tendrá como prioridad la privacidad del derecho a ejercer el voto. Esto se logrará a traves de una desvinculación entre el usuario y el voto ejercido. Es decir, el registro de los votos no proporcionarán información alguna sobre el usuario que ejerció el voto. 
  - Integridad: ITAMPropone será fiel a los datos. Esto se logrará a través de un algoritmo preciso de conteo de votos en el que el voto del usuario cuente una sola vez para cada proyecto. 
  - Disponibilidad: ITAMPropone será accesible para toda la comunidad ITAM que cuente con su correo institucional. Las versiones posteriores se harán públicas, así como las actualizaciones en requerimientos y funcionalidades. Todos los usuarios que utilicen ITAMPropone tendrán acceso a todas las funcionalidades del sistema para las que tengan permiso.
  - Rendición de cuentas: ITAMPropone tendrá u registro detallado de las acciones que realizan los usuarios a través de sus logins. Con esto, podrá garantizar el buen uso del sistema y reportar aquellas cuentas que falten a las políticas.
  
  ### 5.3 Calidad de software
  
  ITAMPropone ofrece a sus usuarios un ambiente simple, eficiente e intuitivo. Las interfaces de ITAMPropone están diseñadas para ser autoexplicativas, tanto para usuarios generales como para administradores. ITAMPropone cumple con todos los requerimientos funcionales, de desempeño, de seguridad y de calidad que se solicitaron en el proyecto final del curso de Ingeniería de Software del Instituto Tecnológico Autónomo de México.
  ITAMPropone garantiza un software de calidad, ya que sigue los principios:
  - Exactitud: ITAMPropone compartirá el resultado de sus estadísticas y votaciones de acuerdo con los datos recaudados.
  - Adaptabilidad: ITAMPropone será accesible para toda la comunidad ITAM.
  - Mantenibilidad: ITAMPropone será manejado por los usuarios administradores, quienes serán capacitados para mantener el software.
  - Disponibilidad: ITAMPropone estará disponible para toda la comunidad ITAM en semestres de Primavera y Otoño.
  - Usabilidad: el diseño intuitivo de ITAMPropone estará dirigido a una experiencia de usuario.
  - Reusabilidad: ITAMPropone permitirá las propuestas de todos los proyectos que la comunidad ITAM quiera aportar. La eliminación de las propuestas estará sujeta a la administración.

  
