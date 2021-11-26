# NullPointerProyectoFinal
Integrantes:
Elisa Espinosa, Jorge Ortiz, Karen Arteaga y Victor Castillejos

ITAMPropone es una aplicación para proponer proyectos al ITAM en dónde les alumnes pueden votar por los mejores proyectos.
Las votaciones por los proyectos que a les estudiantes les interesan se manejan de la siguiente forma. En la pantalla de votaciones aparece una tabla con el nombre y la descripción de cada proyecto. Además, aparece la opción de votar por los proyectos que te gusten, pero solo permite votar una vez por cada uno. 

# Especificación de requerimientos de software

El documento de especificación de requerimientos de software con 3 casos de uso por requerimiento se encuentra en el siguiente enlace:
[Requerimientos de software para ITAMPropone](https://github.com/Ingenieria-de-Software-2021-ITAM/NullPointerProyectoFinal/blob/main/SoftwareRequirementsSpecificationITAMPropone.md)
Los apartados que no se encuentran en el documento de especificación de requerimientos de software se descartaron debido a que la versión actual del producto se encuentra en la fase de prototipo.

## Plan de Calidad

Para garantizar que la pagina ITAMPropone cuente con todos los requerimientos de calidad, se seguira este [Plan de Calidad](https://github.com/Ingenieria-de-Software-2021-ITAM/NullPointerProyectoFinal/blob/main/PlanCalidad.md#plan-de-calidad-para-itampropone). Se busca guardar la confidencialidad de nuestros usuarios mientras se guarda la integridad. Implementaremos medidas que fomenten la disponibilidad a la par de medidas que aseguren la autenticación del usuario. Haremos pruebas para medir y mejorar la fiabilidad y rendimiento de nuestra pagina. Finalmente  cuidaremos que nuestro software sea facil de mantener y entregar, elementos vitales para obtener un producto de calidad.


## Arquitectura

Elegimos una arquitectura combinada spaced-baced y por capas. Estas dos arquitecturas se complementan perfectamente para el desarrollo del sistema ITAMPropone, ya que las desventajas de una son ventajas de la otra.
La arquitectura space-based ofrecerá alta agilidad, fácil despliegue, alta escalabilidad y alto desempeño. La arquitectura por capas ofrecerá facilidad para probar y desarrollar el producto.
En específico, las características que ofrecerá nuestra arquitectura combinada son las siguientes:
- Agilidad: se trabajará en unidades de procesamiento que permitirán el funcionamiento rápido y adaptable. 
- Despliegue: el fácil despliegue de la arquitectura space-based permitirá que se el sistema se despliegue las veces necesarias sin tener problemas. Esto es muy importante en la arquitectura del sistema por la necesida de edsplegar cada vez que se genera un voto.
- Desempeño: el alto desempeño de la arquitectura space-based contrarrestará el bajo desempeño de la arquitectura por capas, pues los mecanismos de almacenamiento de memoria y acceso serán controlados.
- Pruebas: gracias a la arquitectura por capas las el producto será fácil de probar. Esta arquitectura permitirá simular el funcionamiento de capas específicas sin tener que probar el sistema completo.
- Escalabilidad: los módulos de la arquitectura space-based permitirán la escalabilidad que no se logra con la arquitectura por capas. Se trabajará con unidades funcionales que no dependen de las otras para funcionar. 
- Desarrollo: la arquitectura por capas es la más utilizada por su facilidad de desarrollo.

Una aplicación web típica está compuesta por una capa de presentación (funcionalidad relacionada con la interfaz de usuario), una capa de negocios (procesamiento de reglas de negocios) y una capa de datos (funcionalidad relacionada con el acceso a datos). Aplicaciones web Corporativas y sitios Web son ejemplos de esta arquitectura.

## Metodología

Implementamos la metodología AGILE porque utiliza periodos cortos de desarrollo llamado Sprints. Este enfoque permite hacer alteraciones para adaptarse conforme avanza el proyecto. 
Las características por las que elegimos estas metodología sn las siguientes:
- Adaptablidad y cambio de enfoque: esta metodología responde a los cambios de una manera favorable. Con un proyecto ITAMPropone el cambio es inevitable, entonces se necesita una metodología que responda y se adapte al proceso del proyecto. 
- Comunicación directa: la metodología AGILE permitirá que la comunicación entre los integrantes del equipo sea natural y transparente. Esto es muy necesario en nuestro caso por la reducida cantidad de integrantes del equipo.
- Perfeccionamiento: la arquitectura AGILE va a permitir que se mejore el producto y con esto perfeccionar la calidad, completar los objetivos, actualizar las funcionalidades y sacar nuevas versiones del producto.

## Código

El prototipo del preyecto ITAMPropone se encuentre en el siguiente enlace:
https://app.moqups.com/mevbofgFeMiSIqXfxduif6CG89wNGW8F/view/page/af2dcae8a

## Documentación para replicar

  La guía para la visualización del prototipo del sistema ITAMPropone es la siguiente.
  1. Verificar que se cuenta con una conexión de internet estable.
  2. Ingresar al enlace: https://app.moqups.com/mevbofgFeMiSIqXfxduif6CG89wNGW8F/view/page/ad64222d5#
  3. Navegar por el prototipo con los botones que aparecen en pantalla.

## Propuesta económica

[Propuesta económica para ITAMPropone](https://docs.google.com/spreadsheets/d/1X4sJLzmyVvuYx860ZdQr7GSJIlZPPlW4-zG5PzRE7gA/edit#gid=0)
