# Capitulo III: Requirements Specification
## 3.1 To-Be Scenario Mapping
**To-be del segmento grandes empresas de construcción.**

**Preparación de la actividad**

Dibujamos el cuadro y  la dividimos en secciones basándonos en el tipo de contenido que necesitamos incorporar: Fases, Haciendo, Pensando y Sintiendo.

![](/Assets/CHAPTER_II/planificacion.jpg)

**Brainstorming**

Luego de realizar las entrevistas al segmento objetivo, realizamos una lluvia de ideas en cómo debería ser nuestra aplicación para satisfacer las necesidades del cliente

![](/Assets/CHAPTER_II/brainstorming.jpg)

**Identificación de Fases**

Por último, organizamos e identificamos las ideas de las cuales nuestro proyecto si tenia el alcance de resolver las ilustramos en el cuadro, tales como: Planning, Pre-construction, Construction, Monitoring-Control y Ending.

![](Aspose.Words.e458f30a-1693-4682-8ea9-7b943b3f084e.003.png)

**To-be del Contratistas independientes y pequeñas empresas**

**Preparación de la actividad**

Dibujamos el cuadro y  la dividimos en secciones basándonos en el tipo de contenido que necesitamos incorporar: Fases, Haciendo, Pensando y Sintiendo.

![](/Assets/CHAPTER_II/TO-BE-GRAN%20ESCALA.jpg)

**Brainstorming**

Luego de realizar las entrevistas al segmento objetivo, realizamos una lluvia de ideas en cómo debería ser nuestra aplicación para satisfacer las necesidades del cliente

![](/Assets/CHAPTER_II/brainstorming.jpg)

**Identificación de Fases**

Por último, organizamos e identificamos las ideas de las cuales nuestro proyecto si tenia el alcance de resolver las ilustramos en el cuadro, tales como: Planning, Pre-construction, Construction, Monitoring-Control y Ending.

![](/Assets/CHAPTER_II/TO-BE-AUTONOMO.jpg)

### 3.2. **User Stories**
| User Story ID | Titulo | Descripcion | Criterios de Aceptacion |
| ------------- | ------ | ----- | ---- |
| HU001 | Ingreso de Usuarios | Como usuario no identificado en el sistema, quiero iniciar sesión en la aplicación, para lograr acceder a mi cuenta personal. | Escenario N°1: Usuario inicia sesión con sus datos personales Dado que el usuario necesitará registrarse para ingresar por primera vez a la aplicación, deberá completar su información personal básica Cuando el usuario coloca en los campos “Correo electrónico” y “Contraseña” Entonces el sistema le asigna una sesión de usuario| 
| HU002 | Registro de usuario(mayor escala) | Como una gran empresa constructora en proyectos de mayor escala quiero registrarme dentro de la aplicación para gestionar de mejor manera mis proyectos. | Escenario N°1: Crear cuenta. Dado que el usuario constructora se encuentra en sección de "inicio" Cuando el el usuario no se encuentra registrado en la aplicación Entonces al seleccionar “Crear Cuenta” el sistema le redireccionará al registro. Escenario N°2: rellenado de datos correctamente. Dado que el usuario se encuentra en la sección de registro y selecciona la opcion "Aceptar" Cuando el usuario rellene todos los datos correctamente Entonces el sistema registra sus datos ingresados a la base de datos y mostrará "Usted se ha registrado de manera exitosa". | 
| HU003 | Registro de usuario(menor escala) | Como contratista o  empresa constructora en proyectos de menor escala quiero registrarme dentro de la aplicación para gestionar de mejor manera mis proyectos. | Escenario 1: El usuario desea crear una cuenta. Dado que el usuario se encuentra en sección de inicio, Cuando el usuario no se encuentra registrado en el aplicación y al seleccionar “Crear una Cuenta”, Entonces el sistema le redireccionará al registro. Escenario 2: El usuario rellena sus datos correctamente. Dado que el usuario se encuentra en la sección de registro y selecciona la opcion "Aceptar" Cuando el usuario rellena todos los datos correctamente. Entonces el sistema registra los datos ingresados a la base de datos correctamente y mostrará "Usted se ha registrado de manera exitosa". | 
| HU004 | Diseño del sistema | Como administrador de la aplicación quiero que el diseño de la aplicación sea accesible, para lograr que los usuarios identifiquen la plataforma. | Escenario N°1: Elección de colores. Dado que necesitamos que el usuario se familiarice con la aplicación, el administrador aplicará colores atractivos And  usara una buena  Tipografía Escenario N°2: Reconocimiento de la marca del producto. Dado que el administrador quiera que la marca sea reconocida Cuando se ejecuta la aplicación Entonces enfocara la marca a una relación mas personalizada para el usuario. |
| HU005 | Comentarios del usuario | Como usuario quiero hacer comentarios dentro de la aplicación para enviar mi opinión sobre la aplicación. | Escenario N°1: El usuario puede enviar comentarios. Dado que soy un usuario de la aplicación, Cuando quiero expresar mi opinión sobre la aplicación,Entonces quiero poder hacer comentarios dentro de la aplicación.
| HU006 | Gestión de proyectos | Como usuario del sistema, quiero que la aplicación me permita llevar un registro del tiempo invertido en cada proyecto, para poder analizar la rentabilidad de mis proyectos. | Escenario N°1: El usuario puede gestionar sus proyectos. Dado que soy usuario del sistema, Cuando trabajo en un proyecto, Entonces la aplicación debe permitirme llevar un registro del tiempo invertido en cada proyecto, para poder analizar la rentabilidad de mis proyectos. | 
| HU007 | Notificaciones via correo | Como usuario del sistema, quiero poder configurar notificaciones, para poder planificar mi trabajo de manera eficiente y evitar retrasos en la obra. | Escenario N°1: Usuario busca configurar notificaciones. Dado que el sistema mostrará opciones de notificaciones, el usuario podrá configurarlo Cuando el usuario cambie el tono y tiempo que desee que llegue la alarma Entonces el sistema guardara automáticamente esas nuevas modificaciones. | 
| HU008 | Interacción con los usuarios | Como administrador del sistema quiero poder comunicarme con los usuarios, para poder ofrecerles un servicio más personalizado. | Escenario N°1: Usuario recibe el servicio de atención al cliente. Dado que el sistema muestra una sección de atención al cliente  And este busca ayudar al usuario con algunas de sus consultas Cuando el usuario busca respuestas a sus consultas Entonces el sistema le enviara un asesor que le ayude en sus dudas de manera personalizada. | 
| HU009 | Manejo de horarios | Como usuario del sistema, quiero una herramienta de programación que me permita crear horarios detallados para cada proyecto, para poder optimizar el uso de los recursos y minimizar los tiempos de inactividad. | Escenario N°1: El usuario recibe un manejo de usuarios. Dado que soy usuario del sistema, Cuando trabajo en un proyecto, Entonces la aplicación debe permitirme llevar un registro del tiempo invertido en cada proyecto, para poder analizar la rentabilidad de mis proyectos. |
| HU010 | Recomendaciones personalizadas de la aplicación | Como usuario de la aplicación, quiero recibir recomendaciones de la aplicacion para luego. | Escenario N°1: El usuario recibirá recomendaciones de la app. Dado que el usuario este ejecutando la aplicación, el sistema le enviara recomendaciones sobre la gestion de proyectos basados en sus preferencias Cuando recibe recomendaciones de la app Entonces el sistema le enviará las recomendaciones necesarias.
| HU011 | Suscripción plan profesional | Como contratista independiente, quiero poder acceder al plan Professional de BuildSphere para gestionar de manera eficiente proyectos. | Escenario N°1: Usuario recibe una suscripción plan profesional. Dado que soy un contratista independiente, Cuando necesito gestionar proyectos de manera eficiente, Entonces quiero poder acceder al plan Professional de BuildSphere. 
| HU012 | Suscripción plan business. | Como gerente de una gran empresa de construcción, quiero utilizar el plan Business de BuildSphere para coordinar la gestión de múltiples unidades de construcción simultáneamente y la seguridad en todos los proyectos. | Escenario N°1: Usuario recibe una suscripción plan profesional Dado que soy un una gran empresa de construcción, Cuando necesito gestionar proyectos de manera eficiente, Entonces quiero poder acceder al plan Business de BuildSphere.

### 3.3. **Impact Mapping**

## Grandes Empresas
![foto_impact_mapping_grandesv1](https://github.com/Andres2580/OpenSource-Images/blob/5697ecc86cb7c4816bba7a2f91bfb9b93b7475d2/images/Impact%20map-GrandesEmpresasv1.png)

![foto_impact_mapping_grandesv2](https://github.com/Andres2580/OpenSource-Images/blob/5697ecc86cb7c4816bba7a2f91bfb9b93b7475d2/images/Impact%20map-GrandesEmpresasv2.png)

## Pequeñas Empresas
![foto_impact_mapping_pequeñasv1](https://github.com/Andres2580/OpenSource-Images/blob/5697ecc86cb7c4816bba7a2f91bfb9b93b7475d2/images/Impact%20map-Peque%C3%B1asEmpresasv1.png)

![foto_impact_mapping_pequeñasv2](https://github.com/Andres2580/OpenSource-Images/blob/5697ecc86cb7c4816bba7a2f91bfb9b93b7475d2/images/Impact%20map-Peque%C3%B1asEmpresasv2.png)

### 3.4. **Product Backlog**

| #Orden | User Story ID | Titulo | Descripción | Story Points |
| ------------- | ------ | ----- | ---- | ----- |
| 1 | HU001 | Ingreso de usuarios | Como usuario no identificado en el sistema, quiero iniciar sesión en la aplicación, para lograr acceder a mi cuenta personal. | 1 | 
| 2 | HU002 | Registro de usuario(mayor escala). | Como una gran empresa constructora en proyectos de mayor escala quiero registrarme dentro de la aplicación para gestionar de mejor manera mis proyectos. | 3 |
| 3 | HU003 | Registro de usuario(menor escala). | Como contratista o  empresa constructora en proyectos de menor escala quiero registrarme dentro de la aplicación para gestionar de mejor manera mis proyectos. | 3 | 
| 4 | HU004 | Diseño del sistema | Como administrador de la aplicación quiero que el diseño de la aplicación sea accesible, para lograr que los usuarios identifiquen la plataforma. | 8 |
| 5 | HU005 | Comentarios del usuario | CComo usuario quiero hacer comentarios dentro de la aplicación para enviar mi opinión sobre la aplicación. | 5 | 
| 6 | HU006 | Gestión de proyectos | Como usuario del sistema, quiero que la aplicación me permita llevar un registro del tiempo invertido en cada proyecto, para poder analizar la rentabilidad de mis proyectos. | 8 | 
| 7 | HU007 | Notificaciones via correo. | Como usuario del sistema, quiero poder configurar notificaciones, para poder planificar mi trabajo de manera eficiente y evitar retrasos en la obra. | 5 |
| 8 | HU008 | Interacción con los usuarios | Como administrador del sistema quiero poder comunicarme con los usuarios, para poder ofrecerles un servicio más personalizado. | 3 | 
| 9 | HU009 | Manejo de horarios | Como usuario del sistema, quiero una herramienta de programación que me permita crear horarios detallados para cada proyecto, para poder optimizar el uso de los recursos y minimizar los tiempos de inactividad. | 3 |
| 10 | HU010 | Recomendaciones personalizadas de la aplicación | Como usuario de la aplicación, quiero recibir recomendaciones de la aplicación para luego usarlos. | 5 |
| 11 | HU011 | Suscripción plan profesional | Como contratista independiente, quiero poder acceder al plan Professional de BuildSphere para gestionar de manera eficiente proyectos.| 5 |
| 12 | HU012 | Suscripción plan business | Como gerente de una gran empresa de construcción, quiero utilizar el plan Business de BuildSphere para coordinar la gestión de múltiples unidades de construcción simultáneamente y la seguridad en todos los proyectos. | 5 |
| 13 | HU013 | Proyectos |Como usuario de BuildSphere, Quiero poder crear un nuevo proyecto de construcción, para gestionar y dar seguimiento a las actividades y recursos relacionados con el proyecto. | 5 |
