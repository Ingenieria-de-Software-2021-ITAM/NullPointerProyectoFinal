# Plan de calidad para ITAMPropone
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
1) [Identificador de plan de calidad](#identificador)
2) [Referencias](#Referencias)
3) [Introducción](#Introduccion)
4) [Objetos de Prueba](#Objetos)
5) [Eventos de riesgo del software ](#Eventos-de-riesgo)
6) [Funcionalidades a probar ](#Funcionalidades)
7) [Funcionalidades que no se probaran ](#Funcionalidades-no )
8) [Acercamiento](#Acercamiento)
9) [Criterios de eventos exitosos o fallidos ](#Criterios)
10) [Suspensión de criterios y requerimientos para continuar  ](#Suspension)
11) [Pruebas entregables](#Pruebas)
12) [Tareas de prueba pendientes ](#Tareas)
13) [Necesidades del ambiente](#ambiente)
14) [Necesidades de entrenamiento y staff](#entrenamiento)
15) [Responsabilidades](#Responsibilidades)
16) [Itinerario](#Itinerario)
17) [Riesgos de planeación](#Riesgos)
18) [Aprobaciones](#Aprobaciones)
19) [Glosario](#Glosario)
 
## 1.Identificador de plan de calidad <a name="identificador"></a>
Versión 1.0 del Master Plan

## 2.Referencias <a name="Referencias"></a>

[ITAMPropone prototipo (versión actual)](https://app.moqups.com/mevbofgFeMiSIqXfxduif6CG89wNGW8F/view/page/af2dcae8a)

[Repositorio en GitHub](https://github.com/Ingenieria-de-Software-2021-ITAM/NullPointer-Markdown)

[Formato del plan de calidad](https://jmpovedar.files.wordpress.com/2014/03/ieee-829.pdf)


## 3.Introducción <a name="Introduccion"></a>
Para garantizar que la página ITAMPropone cuente con todos los requerimientos de calidad, se seguirá este plan de calidad, el cual es nuestro Master Plan. Se busca garantizar la confidencialidad de nuestros usuarios mientras se guarda la integridad. Implementaremos medidas que fomenten la disponibilidad a la par de medidas que aseguren la autenticación del usuario. Haremos pruebas para medir y mejorar la fiabilidad y rendimiento de nuestra página. Finalmente  cuidaremos que nuestro software sea fácil de mantener y entregar, elementos vitales para obtener un producto de calidad.

## 4.Objetos de Prueba <a name="Objetos"></a>
- Inicio de sesión correcto, tanto para administradores como para usuarios
- Redirección apropiada entre las páginas
- Registro de proyectos con datos e imágenes efectivo
- Registro de votos exitoso
- Vista y análisis de datos certeros e intuitivos

## 5.Eventos de riesgo del software <a name="Eventos-de-riesgo"></a>
Las áreas críticas que encontramos que debes probar son:
- Adaptabilidad a distintos navegadores web y distintos dispositivos
- Funciones complejas de autenticacion de usuarios
- Documentación cuidadosa de todo el código
- Implementación de nuevas herramientas para hacer más responsiva la página

Los riesgos inherentes del software que tenemos que cuidar son:
- Regulaciones escolares
- Impacto en los alumnos
- Seguridad

## 6.Funcionalidades a probar <a name="Funcionalidades"></a>
- Ingreso a la página
- Dar de alta un proyecto
- Editar mis proyectos
- Votar por mis proyectos favoritos
- Rechazar los proyectos que no me llamen la atención
- Buscar proyectos que ya haya visto con anterioridad

## 7.Funcionalidades que no se probaran <a name="Funcionalidades-no"></a>
- Enviar mensaje al creador del proyecto
- Dejar comentarios en los proyectos para que otros usuarios los puedan ver
- Ver cuantos likes ha recibido un proyecto
- Incluir videos en la descripción del proyecto
-
## 8.Acercamiento <a name="Acercamiento"></a>
Para realizar nuestras pruebas utilizaremos Manual testing para checar que el software
cumpla con todos los requerimientos, manteniendo como mentalidad el  “qué esperaría el cliente que pase sí hace x o y”. También utilizaremos dinámicos pues creemos que así priorizaremos al cliente, ya que recibirá lo que se esperaba del software. Finalmente utilizaremos Black Box Testing para realizar pruebas de usuarios que nos indiquen si la aplicación es intuitiva y responsiva en escenarios lo más parecidos a cuando se publique la página.

## 9.Criterios de eventos exitosos o fallidos <a name="Criterios"></a>
- Haber realizado todas las pruebas ya programadas
- Tener un éxito del 95 %
-  Ningún error de código mediano con soluciones rápidas o que pueda llevar próximamente al fallo de la página

## 10.Suspensión de criterios y requerimientos para continuar <a name="Suspension"></a>
En caso de surgir algún error que pueda llevar a fallo la página, suspenderemos las pruebas y regresaremos a trabajar en el código. De igual manera, si en las pruebas de usuario más del 20% de los usuarios se toman más de 15 min en subir un proyecto, declaramos que el sistema no es intuitivo y tendremos que generar otra versión.
 
## 11.Pruebas entregables <a name="Pruebas"></a>

- Documento del plan de calidad
- Casos de prueba
- Especificaciones del diseño de las pruebas


## 12.Tareas de prueba pendientes <a name="Tareas"></a>
- Bitácora de errores y bitácora de ejecución
- Reporte sobre problemas y medidas a implementar

## 13.Necesidades del ambiente <a name="ambiente"></a>
Debemos de realizar al menos 6 pruebas de usuario midiendo el tiempo que les toma realizar cada tarea y si es que necesitan ayuda para lograr su objetivo

## 14.Necesidades de entrenamiento y staff <a name="entrenamiento"></a>
Entrenamiento para todos los integrantes del equipo para utilizar mockups correctamente
Todos los miembros del equipo serán responsables de realizar pruebas de usuario y de realizar las pruebas definidas

## 15.Responsibilidades <a name="Responsibilidades"></a>

El encargado de cada tarea es:
- Definir riesgos: Jorge
- Seleccionar requerimientos a checar y requerimientos que no serán checados: Elisa
- Definicion de estrategia general: Victor
-Asegurarse de que todos los elementos de las pruebas sean correctos: Karen

## 16.Itinerario <a name="Itinerario"></a>
La definición de las pruebas se realizará antes del 26 de noviembre
Las pruebas de usuario estarán listas para el 27 de noviembre del 2021
La corrección de errores se terminará el 6 de diciembre

## 17.Riesgos de planeación <a name="Riesgos"></a>
- Falta de personal para realizar las pruebas
- Entrega tardía del software
- Cambios al diseño y requerimientos originales

## 18.Aprobaciones <a name="Aprobaciones"></a>
Para dar como completo el proceso de pruebas, se deberá de dar el visto bueno por al menos 3 integrantes. En caso de no ser así, se discutirá el porqué de la decisión y se realizará una nueva votación o se continuará trabajando en el proyecto

## 19.Glosario <a name="Glosario"></a>
- RB: Biblioteca Raul Bailleres
- la H: El ITAM
- ITAM: Instituto de Técnicas y Artes de México
 
 

