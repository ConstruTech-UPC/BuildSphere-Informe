# Capítulo V: Product Implementation, Validation & Deployment.

## 5.1. Software Configuration Management.

### 5.1.1. Software Development Environment Configuration.
En esta sección se describirán los productos para el desarrollo de software que han sido implementados para este proyecto. Así mismo, esta sección da su importancia al contar con información relevante para futuros equipos de desarrollo que deseen continuar con el ciclo de vida del producto de software.
### Project Management
- [**Google Meet**](https://meet.google.com/): Plataforma que funciona como aplicación web y mobile. Se empleó esta plataforma como medio para las reuniones virtuales, las diversas ceremonias de SCRUM con el equipo.
- [**Trello**](https://trello.com/es): La herramienta es una aplicación web empleada para realizar la asignación de tareas en el formato (do, doing & done). De tal forma que todo el equipo tenga conocimiento de las tareas que se están realizando con el fin de tener un buen proyecto.
### Requirements Management
- [**Trello**](https://trello.com/es): La herramienta nos permite realizar un backlog de equipo y colaborar en el mismo. Adicionalmente, proporciona una vista cómoda respecto a este dejando en claro los puntos de interés o prioridad del equipo.
### Product UI/UX Design
- [**Figma**](https://www.figma.com/): La aplicación web de Figma fue utilizada para desarrollar los wireframes, mockups y mobile applications prototyping de manera colaborativa.
- [**Uxpressia**](https://uxpressia.com/): Se empleó esta aplicación web para la realización de los User Personas, el Customer Journey Map, Empathy Map e Impact Map.
- [**Miro**](https://miro.com/): La aplicación web de Miro ha sido utilizada en el desarrollo de los escenarios mapping y customer journey map
### Software Development
- **Landing Page**: Para la realización del landing page se utilizarán las tecnologías de: HTML5, CSS3 y JavaScript. Además, para realizar un óptimo desarrollo para la forma responsiva, se utilizará el framework de BootStrap.
- **Frontend Web Application**: Para la realización del está sección de nuestra aplicación web se usarán las mismas tecnologías que en el Landing Page. Adicionalmente, nos estaremos apoyando del framework Angular para su realización como librería complementaria de JavaScript.
- **Herramientas:** Node, npm, ng
### Web Services
Para los diversos servicios web que se desarrollaran, se empleará el estilo de arquitectura RESTful API. Se usará el lenguaje JAVA, ya que estaremos usando SPRINT BOOT.
### IDE's de desarrollo
[**Webstorm**](https://www.jetbrains.com/webstorm/): Este IDE será usado para el desarrollo de la parte del frontend de la aplicación web.

[**IntelliJ IDEA Ultimate**](https://www.jetbrains.com/es-es/idea/): Este IDE será usado para el desarrollo de la parte del backend de la aplicación web.
### Software Testing
Para realizar pruebas del landing page y la aplicación web, se utilizaron los principlaes navegadores web como [Google Chrome]([https://www.google.com/chrome/](https://www.google.com/chrome/)), [Microsoft Edge]([https://www.microsoft.com/en-us/edge](https://www.microsoft.com/en-us/edge)) y [Mozilla Firefox]([https://www.mozilla.org/en-US/firefox/new/](https://www.mozilla.org/en-US/firefox/new/)).
Adicionalmente, se usará la extensión [Google Lighthouse]([https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk](https://chrome.google.com/webstore/detail/lighthouse/blipmdconlkpinefehnmjammfjpmpbjk))para tener un panorama automatizado y actualizado del landing page.
### Project Deployment
[**Vercel**](https://vercel.com/): Para llevar a cabo el deployment del landing page, se procedió a vincular el repositorio de Github con Netlify. De este modo, Netlify gestionará de manera automática el deploy del landing page cada vez que exista un nuevo cambio en el repositorio.

[**Netlify**](https://www.netlify.com/): Para llevar a cabo el deployment del front-end, se procedió a vincular el repositorio de Github con el servicio de Vercel. De este modo, el despliegue de la página será de manera óptima.
### Software Documentation
- [**GitHub**](https://github.com/): Para la realización del informe y diversos entregables, se ha creado un repositorio en el formato markdown para tener un control de versiones de los archivos.
- [**Lucidchart**](https://www.lucidchart.com/): Aplicación web que fue utilizada para el desarrollo de los wireflows, user flows y diagramas UML.
- [**Structurizr**](https://structurizr.com/): Aplicación web que fue utilizada para  crear los diagramas C4 de manera sencilla.
### 5.1.2. Source Code Management.
El manejo y la organización de las diferentes modificaciones se llevaron a cabo mediante la plataforma de gestión de repositorios Github.
#### Organización:
[ConstruTech-UPC](https://github.com/ConstruTech-UPC)
![](https://lh7-us.googleusercontent.com/Zi13t8pIT3exNojOJXOe4K7YSeR668wkDM4K6KGQ3bNvIK4-Z2L58sCzsltOvz9r6LNryRmX8TVV5NWIZSEkCsgXuGSfT5rI2tgnM_JZZh2Fx44R4DTJ-XXuR9VHa2bWLnnvjIBp8uSBDwek7gGWy1U)
#### Repository:
- [Informe](https://github.com/ConstruTech-UPC/BuildSphere-Informe)
- [Landing Page](https://github.com/ConstruTech-UPC/BuildSphere-Landing-Page)
- [Acceptance test](https://github.com/ConstruTech-UPC/BuildSphere-acceptance-tests)
#### Control de versiones con GitFlo:w:
Para llevar un control de las ramas, los commits y los cambios realizados en el código fuente, se procedió a utilizar GitFlow.
Se tenían las siguientes ramas en cada repositorio:
- main: En esta rama se almacenan las versiones oficiales del repositorio que ya deben pasar a producción.
- develop: Esta rama se utiliza como rama de integración para las "feature branches". Una vez el "head" alcance un estado estable y el equipo lo considere listo para ser lanzado, se unirá a la rama release.
- feature: En estas ramas se trabajan las features que se unirán a la rama develop.
- release: En wsta rama se podrá corregir pequeños bugs.

##### Convenciones de Commits
El formato de nuestros commits sigue la estructura de los "Conventional Commits" en su versión [1.0.0]([https://www.conventionalcommits.org/en/v1.0.0/](https://www.conventionalcommits.org/en/v1.0.0/)) con el siguiente formato:

``<type>[optional scope]: <description>

Donde:
- type: Indica el tipo de cambio realizado en el commit. Los tipos más comunes son:
- feat: Nueva característica
- fix: Corrección de un bug
- chore: Tareas de mantenimiento
- docs: Actualización de la documentación
- scope: (opcional) Indica el área del código que ha sido modificada.
- description: Breve descripción del cambio realizado.

Ejemplo de commit:

`feat: Implementación del componente de 'add new comic'`
### 5.1.3. Source Code Style Guide & Conventions.
**HTML/CSS Style Guide**

Para nuestro proyecto, hemos decidido seguir el Google HTML/CSS Style Guide([Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html)) y HTML Style Guide([HTML Style Guide and Coding Conventions (w3schools.com)](https://www.w3schools.com/html/html5_syntax.asp)) de w3Scholls , garantizando así un código claro y coherente que se alinea con las mejores prácticas de la industria. Dentro de las convenciones de esta guía de estilo que adoptaremos se encuentran:

- General:
    - Nos aseguramos de usar siempre HTTPS para recursos embebidos para mejorar la seguridad. Adoptamos una indentación consistente de dos espacios, evitando mezclar espacios con tabulaciones, y mantenemos todo el código en minúsculas, incluidos nombres de elementos, atributos y selectores. Además, eliminamos los espacios en blanco al final de las líneas para facilitar la revisión del código.
- Metadatos Generales:
    - En nuestros documentos, utilizamos la codificación UTF-8 sin marca de orden de bytes, especificada con meta charset="utf-8".
- Reglas de Estilo HTML:
    - Adoptamos HTML5 como tipo de documento estándar, según lo recomendado por Google. Nos aseguramos de que nuestro HTML sea válido para mantener una calidad de código medible. Usamos elementos HTML según su propósito, como < p> para párrafos y < a> para enlaces, lo cual es importante para la accesibilidad y la eficiencia del código. Mantenemos una clara separación entre la estructura, la presentación y el comportamiento, delegando la presentación al CSS y el comportamiento a los scripts.
- Reglas de Estilo CSS:
    - Nos adherimos a las directrices de Google para utilizar CSS válido y seleccionar nombres de clases que reflejan el propósito del elemento en lugar de nombres presentacionales. Preferimos las propiedades en forma abreviada y omitimos las unidades después de los ceros cuando no son necesarias, lo que mejora la eficiencia y la comprensibilidad del código. También evitamos los selectores de ID para prevenir conflictos y mantener una especificidad manejable.
- Formato CSS:
    - Consideramos ordenar las declaraciones CSS alfabéticamente para mejorar la coherencia y mantenibilidad. Aseguramos que cada selector y declaración comience en una nueva línea y separamos cada bloque de reglas claramente con líneas en blanco, lo que facilita la lectura y la edición del código.


**Gherkin Style Guide**

Para la escritura de los *acceptance test* en nuestro proyecto, seguiremos el Gherkin Style Guide([Make your Gherkin Specifications More Readable (specflow.org)](https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/)) hecho por SpecFlow. Esto garantizará que nuestros tests sean claros y mantenibles, facilitando la colaboración y comprensión entre los miembros del equipo y asegurando una alta calidad en nuestras pruebas.

- Discernible Given-When-Then Blocks:
    - Utilizaremos la indentación para separar claramente los bloques Given-When-Then. Los pasos adicionales marcados con "And" se indentarán para mantener la legibilidad y distinguir fácilmente el inicio y fin de cada sección.
- Steps with Tables:
    - Para pasos que incluyan tablas, emplearemos dos puntos al final de cada paso para indicar la presencia de datos tabulados. Esto mantendrá nuestras especificaciones ordenadas y facilitará la identificación de los datos requeridos.
- Reducing Noise:
    - Minimizamos el ruido en nuestros escenarios utilizando valores predeterminados para campos irrelevantes al contexto del test. Esto mantendrá el enfoque en los aspectos importantes y mejorará la claridad de nuestros tests.
- Parameters in Steps:
    - Destacaremos los parámetros dentro de los pasos utilizando comillas simples. Esto ayudará a identificar rápidamente los parámetros y sus valores esperados en cada paso de nuestros escenarios.
- Newlines within Scenarios:
    - Incorporaremos líneas nuevas para separar lógicamente las unidades de información dentro de nuestros escenarios. Esto ayudará a agrupar pasos relacionados y mejorará significativamente la legibilidad.
- Newlines between scenarios and separator comments:
    - Añadiremos dos líneas nuevas y comentarios separadores entre escenarios para facilitar la navegación visual en los archivos de características. Estos separadores nos ayudarán a identificar rápidamente dónde termina un escenario y comienza otro.

**Angular Style Guide**

Para el desarrollo de la parte front-end de nuestra aplicación web, seguiremos el Angular coding style guide([Angular - Angular coding style guide](https://angular.io/guide/styleguide#toc)). Esto garantizará que nuestro código sea consistente y siga las mejores prácticas establecidas por la comunidad Angular, facilitando así el mantenimiento y la escalabilidad de nuestra aplicación. Además, promoveremos una estructura clara y modular que permita a cualquier miembro del equipo comprender y contribuir eficientemente al proyecto. En resumen, haremos usos de estas convenciones.

- Estructura de archivos y responsabilidad única:
    - Cada componente, servicio u otro símbolo debe definirse en su propio archivo, preferiblemente limitado a 400 líneas de código para facilitar el mantenimiento. Separaremos la lógica de arranque de la aplicación en un archivo main.ts, manteniendo los archivos de aplicación lo más limpios posible.
- Funciones pequeñas:
    - Definiremos funciones pequeñas que no superen las 75 líneas para promover la reutilización y facilitar las pruebas y el mantenimiento.
- Convenciones de nomenclatura:
    - Usaremos nombres consistentes para todos los símbolos, siguiendo el patrón de característica.tipo.ts. Para los selectores de componentes y directivas, usaremos kebab-case y un prefijo personalizado que identifique la característica o la aplicación en sí.
- Módulos de Angular:
    - Crearemos un NgModule para cada característica distintiva de la aplicación, colocándolos en carpetas con nombres que reflejen la característica que representan.
- Estructura de carpetas por funcionalidad:
    - Organizaremos el código en carpetas basadas en características para facilitar la localización e identificación del código a simple vista. Esto nos ayudará a mantener una estructura plana y manejable.
- Módulo raíz de la aplicación y módulos de características:
    - El módulo raíz de la aplicación se llamará app.module.ts y cada módulo de características llevará el nombre de la característica que define, como machines.module.ts para una característica de maquinarias.
- Módulos compartidos:
    - Utilizaremos un SharedModule para declarar componentes, directivas y pipes que se reutilizarán en todo el proyecto, evitando proporcionar servicios en este módulo para no generar instancias separadas en módulos con carga diferida.
- Servicios como singletons:
    - Implementaremos servicios como singletons dentro del mismo inyector para compartir datos y funcionalidades. Estos servicios tendrán responsabilidades únicas y se les proporcionará en el inyector raíz de la aplicación.
- Decoradores de propiedad de entrada y salida:
    - Usaremos los decoradores @Input() y @Output() para las propiedades de entrada y salida de los componentes en lugar de las propiedades inputs y outputs de los metadatos @Directive y @Component.
- Lógica de presentación:
    - Mantendremos la lógica de presentación en la clase del componente, extrayendo plantillas y estilos a sus propios archivos cuando superen las 3 líneas para mantener la legibilidad y la capacidad de mantenimiento.

**Java Style Guide**

Para el uso de buenas prácticas de codificación en Java, seguiremos la Guía de Estilo de Google para Java ([Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)), asegurando así la claridad y consistencia en nuestro código. A continuación se detallan las convenciones clave que aplicaremos:

- Estructura de archivos de origen:
    - Cada archivo de código fuente llevará el nombre de la clase de nivel superior que contiene y estará codificado en UTF-8.
    - Se utilizarán secuencias de escape para caracteres especiales, optando por caracteres Unicode cuando aumente la legibilidad.
- Estructura de archivos fuente:
    - Cada archivo contendrá una declaración de paquete sin ajuste de línea.
    - Evitaremos las importaciones con comodines, manteniendo todas las declaraciones de importación sin ajuste de línea y agrupadas según corresponda.
- Formateo:
    - Incrementaremos la indentación en bloques en +2 espacios y continuaremos las líneas en al menos +4 espacios.
    - Mantendremos un límite máximo de 100 caracteres por línea, aplicando ajuste de línea donde sea necesario.
- Nombramiento:
    - Todos los identificadores usarán solo letras ASCII y números, evitando guiones bajos, prefijos o sufijos especiales.
    - Nombraremos las clases con UpperCamelCase, los métodos con lowerCamelCase, y las constantes con UPPER\_SNAKE\_CASE.
- Prácticas de programación:
    - Siempre usaremos la anotación @Override cuando sea legal hacerlo.
    - Nunca ignoraremos las excepciones capturadas, optando por registrarlas o manejarlas como corresponda.
- Javadoc:
    - Proporcionaremos Javadoc para todas las clases públicas y miembros protegidos o públicos, con excepciones para miembros autoexplicativos y anulaciones.
    - Cada bloque de Javadoc comenzará con un breve resumen, escrito como un fragmento y no como una oración completa
- Otro:
    - Formateamos las clases enum de manera que sean claras y organizadas, separando constantes con comas y permitiendo saltos de línea opcionales.
    - Colocaremos anotaciones directamente antes del tipo que anotan y en su propia línea para las clases.

**TypeScript Style Guide**

Para el lenguaje de programación TypeScript que se utilizará en el entorno front-end, seguiremos las directrices de estilo proporcionadas por la guía de estilo de TypeScript de Google([Google TypeScript Style Guide](https://google.github.io/styleguide/tsguide.html)). Aquí hay un resumen de las convenciones clave:

- Fundamentos del archivo de código fuente:
    - Los archivos TypeScript deben estar codificados en UTF-8 y contener únicamente el carácter de espacio horizontal ASCII, exceptuando la secuencia de terminación de línea. Las secuencias de escape especiales deben ser utilizadas en lugar de las numéricas o Unicode, y para caracteres no ASCII se recomienda usar el carácter Unicode real junto con un comentario explicativo.
- Estructura del archivo fuente:
    - ​​Un archivo TypeScript se compone de información de derechos de autor, un JSDoc de resumen del archivo cuando corresponda, seguido por las secciones de importaciones y finalmente, la implementación del código.
- Importaciones:
    - Se deben manejar con cuidado, usando la sintaxis de ES6 y TypeScript apropiadamente. Se prefieren las importaciones nombradas sobre las de espacios de nombres para evitar la introducción de muchos símbolos distintos desde grandes APIs.
- Tipos:
    - Se debe confiar en la inferencia de tipos del compilador para todos los tipos de expresiones siempre que sea posible. Sin embargo, si el tipo no es obvio a partir del contexto, se deben proporcionar anotaciones de tipo explícitas para mayor claridad.
- Control de flujo:
    - Los bloques de control de flujo siempre deben usar llaves, incluso si contienen solo una declaración. Esto mejora la legibilidad y mantiene la consistencia del código.
- Control de excepciones:
    - Los bloques try-catch deben utilizarse para manejar casos excepcionales y se debe explicar con comentarios cuando se elige no tomar ninguna acción en un bloque catch.
- Declaraciones de funciones y métodos:
    - Prefiera declaraciones de funciones para funciones nombradas y utilice funciones flecha para funciones anónimas o callbacks. Evite la asignación dentro de las declaraciones de control si se puede realizar fuera de ellas.
- Herramientas del compilador TypeScript:
    - Todos los archivos deben ser verificados y aprobados por el compilador de TypeScript sin errores para asegurar la integridad del código.
- Comentarios y documentación:
    - Utilice comentarios de estilo JSDoc para documentar el código que será utilizado por otros y comentarios de una sola línea para notas relacionadas con la implementación interna del código. Todos los símbolos exportados deben estar adecuadamente documentados.
- Convenciones y nomenclatura:
    - Los identificadores deben seguir las convenciones de UpperCamelCase para clases y tipos y lowerCamelCase para variables y funciones. Evite los prefijos y sufijos de guiones bajos y use nombres descriptivos y claros.
- Formato del código:
    - Sea coherente con el uso de puntos y comas y siga las convenciones de formato establecidas para mantener la legibilidad y estructura del código.
- Prácticas generales:
    - Evite el uso de características no estándar de ECMAScript y la modificación de los objetos integrados para mantener la compatibilidad y la claridad del código en toda la base de código.

**Spring Boot Style Guide**

Para el lenguaje de programación TypeScript que se utilizará en el entorno front-end, seguiremos las directrices de estilo proporcionadas por la guía de estilo de TypeScript de Google([Google TypeScript Style Guide](https://google.github.io/styleguide/tsguide.html)). Aquí hay un resumen de las convenciones clave:

- Inicio automatizado: Usaremos la clase SpringApplication para iniciar nuestra aplicación desde el método main(). Este método estático arrancará la aplicación, creará el contexto de la aplicación y configurará los beans predeterminados.
- Información de Inicio: Configuraremos la aplicación para que al iniciar, se muestre información útil como la versión de la aplicación, los perfiles activos y la inicialización del servidor web, aprovechando la salida de registro a nivel INFO.
- Manejo de Fallos de Inicio: En caso de fallos de inicio, como puertos ocupados, Spring Boot nos ayudará a diagnosticar y corregir problemas con mensajes de error específicos y acciones sugeridas a través de sus analizadores de fallos.
- Inicialización Perezosa: Podemos optar por habilitar la inicialización perezosa para mejorar el tiempo de inicio de la aplicación. Esto pospondrá la creación de los beans hasta que se necesiten realmente, lo cual es útil durante el desarrollo y en entornos de prueba.
- Personalización del Banner: Personalizaremos el banner que se muestra al inicio para reflejar la identidad de nuestro proyecto. Podemos incluir información útil o simplemente estilizar la salida en la consola para mejorar la experiencia del desarrollador.
- Configuración Personalizada: A través de una instancia de SpringApplication personalizada, tendremos la posibilidad de modificar la configuración predeterminada, como deshabilitar el banner de arranque si es necesario.
- API Constructora Fluida: Utilizaremos SpringApplicationBuilder en situaciones en las que necesitemos construir jerarquías de contextos de aplicación o si preferimos una API fluida para configurar nuestra aplicación.
- Eventos y Escuchadores de Aplicación: Registraremos escuchadores de eventos de aplicación que nos permitan ejecutar acciones específicas en momentos críticos del ciclo de vida de la aplicación.
- Entorno Web: SpringApplication configurará automáticamente el tipo de ApplicationContext apropiado, asegurando que tengamos todas las funcionalidades necesarias para un entorno web completo.
- Argumentos de la Aplicación: Accederemos a los argumentos de línea de comandos dentro de la aplicación utilizando ApplicationArguments para ajustar el comportamiento de la aplicación en tiempo de ejecución según sea necesario.
- Ejecución de Código Post-Inicio: Implementaremos ApplicationRunner o CommandLineRunner para ejecutar cualquier configuración o lógica de inicialización que necesite tener lugar justo después de que la aplicación haya arrancado.
- Salida de la Aplicación: Aseguraremos una salida y limpieza elegantes del contexto de la aplicación cuando se cierre, mediante el gancho de apagado que SpringApplication registra en la JVM.

## 5.1.4. Software Deployment Configuration.
Para el despliegue de nuestra Landing Page utilizamos la aplicación Vercel, esta plataforma permite a los desarrolladores contruir, desplegar y esscalar aplicaciones front-end sin necesidad de servidores. Decidimos usar esta plataforma debido a la facilidad que nos brinda, solo necesitamos colocar el repositorio de nuestra Landing Page para que la despliegue sin problemas, es un proceso automatizado y rápido.

# 5.2. Landing Page, Services & Applications Implementation.
## 5.2.1. Sprint 1
## 5.2.1.1 Sprint Planning 1
<table>
  <tr>
    <td align="center"><strong>Sprint #</strong></td>
    <td align="center"><strong>1</strong></td>
  </tr>
  <tr>
  <td colspan="2" align="center"><strong>Sprint Planning Background</strong></td>
  </tr>
  <tr>
    <td align="center">Date</td>
    <td align="center">2024/04/07</td>
  </tr>
  <tr>
    <td align="center">Time</td>
    <td align="center">11:00 AM</td>
  </tr>
  <tr>
    <td align="center">Location</td>
    <td align="center">Modalidad virtual, uso de Google Meets</td>
  </tr>
  <tr>
    <td align="center">Prepared By</td>
    <td align="center">Camila Cristina Loli Ramirez</td>
  </tr>
  <tr>
    <td align="center">Attendees (to planning meeting)</td>
    <td align="center">Alvaro Esteban Crispin Ccancce<br>Camila Cristina Loli Ramirez<br>Carlos Andres Rojas Ccama<br>Eduardo Renato Ventura Chancafe<br>Piero Mendoza Pimentel</td>
  </tr>
  <tr>
    <td align="center">Sprint 2 – 1 Review Summary</td>
    <td align="center">No hay Sprints anteriores, por lo tanto, no aplica. </td>
  </tr>
  <tr>
    <td align="center">Sprint 2 – 1 Retrospective Summary</td>
    <td align="center">En esta reunión hemos divido las respectivas responsabilidades de cada integrante para el cumplimiento del Capítulo 5, que incluye la Landing Page, y algunas modificaciones de los capítulos previos. Asimismo, estuvimos conversando sobre las posibles herramientas a usar para la creación de la Landing Page y el despliegue.</td>
  </tr>
  <tr>
    <td colspan="2" align="center"><strong>Sprint Goal & User Stories</strong></td>
  </tr>
  <tr>
    <td align="center">Sprint 1 Goal</td>
    <td align="center">Se debe completar el informe con los cinco capítulos y la respectiva Landing Page</td>
  </tr>
  <tr>
    <td align="center">Sprint n Velocity</td>
    <td align="center">18</td>
  </tr>
  <tr>
    <td align="center">Sum of Story Points</td>
    <td align="center">18</td>
  </tr>
</table>

## 5.2.1.2 Sprint Backlog 1


<table><tr><th colspan="2" valign="top">Sprint #</th><th colspan="6" valign="top">Sprint 1</th></tr>
<tr><td colspan="2" valign="top">User story</td><td colspan="6" valign="top">Work Item/ Task</td></tr>
<tr><td valign="top"><b>Id</b></td><td valign="top"><b>Title</b></td><td valign="top"><b>Id</b></td><td valign="top"><b>Title</b></td><td valign="top"><b>Description</b></td><td valign="top"><b>Estimation(hours)</b></td><td valign="top"><b>Assigned to</b></td><td valign="top"><b>Status(To-do /InProcess To Review Done)</b></td></tr>
<tr><td rowspan="2" valign="top">US01/EPIC 01</td><td rowspan="2" valign="top"><p><b>Implementación de Barra de navegación</b></p><p></p></td><td valign="top">C01</td><td valign="top">Navbar section</td><td valign="top">Hacer barra de navegación con link internos a cada sección de la landing page</td><td valign="top">1</td><td valign="top">Alvaro</td><td valign="top">Done </td></tr>
<tr><td valign="top">C02</td><td valign="top">Responsive design navbar section</td><td valign="top"></td><td valign="top">1</td><td valign="top">Alvaro</td><td valign="top">Done </td></tr>
<tr><td rowspan="2" valign="top">US02 / EPIC 01</td><td rowspan="2" valign="top">Logo y Descripción de la empresa</td><td valign="top">C03</td><td valign="top">Hero section</td><td valign="top"></td><td valign="top">1</td><td valign="top">Alvaro</td><td valign="top">Done </td></tr>
<tr><td valign="top">C04</td><td valign="top">Responsive design hero section</td><td valign="top"></td><td valign="top">1</td><td valign="top">Alvaro</td><td valign="top">Done </td></tr>
<tr><td rowspan="2" valign="top">US03 / EPIC 01</td><td rowspan="2" valign="top">Visión y Misión de la empresa</td><td valign="top">C05</td><td valign="top">About us section</td><td valign="top"></td><td valign="top"></td><td valign="top">Eduardo Ventura</td><td valign="top"></td></tr>
<tr><td valign="top">C06</td><td valign="top">Responsive design about us section </td><td valign="top"></td><td valign="top"></td><td valign="top">Eduardo Ventura</td><td valign="top"></td></tr>
<tr><td rowspan="2" valign="top">US04 / EPIC01</td><td rowspan="2" valign="top">Detalles y Servicios de la empresa</td><td valign="top">C07</td><td valign="top">Features section</td><td valign="top"></td><td valign="top"></td><td valign="top">Eduardo Ventura</td><td valign="top"></td></tr>
<tr><td valign="top">C08</td><td valign="top">Responsive design features section</td><td valign="top"></td><td valign="top"></td><td valign="top">Eduardo Ventura</td><td valign="top"></td></tr>
<tr><td rowspan="2" valign="top">US05 / EPIC01</td><td rowspan="2" valign="top">Contacto con un asesor</td><td valign="top">C09</td><td valign="top">Contact us section</td><td valign="top">Hacer el formulario de contacto</td><td valign="top">5h</td><td valign="top">Piero</td><td valign="top">Done</td></tr>
<tr><td valign="top">C10</td><td valign="top">Responsive design features section</td><td valign="top">Añadir el diseño responsive al formulario para que se adapte al tamaño de la pantalla</td><td valign="top">5h</td><td valign="top">Piero</td><td valign="top">Done</td></tr>
<tr><td rowspan="2" valign="top">US06 / EPIC01</td><td rowspan="2" valign="top">Descripción de Planes de suscripción</td><td valign="top">C11</td><td valign="top">Mission and vision section</td><td valign="top">Añadir la sección de la Mision y Vision de la Landing Page</td><td valign="top">2h</td><td valign="top">Camila</td><td valign="top">Done</td></tr>
<tr><td valign="top">C12</td><td valign="top">Responsive design mission and vision section</td><td valign="top">Añadir el responsive design de la seccion Mision y Vision</td><td valign="top">2h</td><td valign="top">Camila</td><td valign="top">Done</td></tr>
<tr><td rowspan="2" valign="top">US07 / EPIC01</td><td rowspan="2" valign="top">Compra de planes de suscripción</td><td valign="top">C13</td><td valign="top">Subscription plans section</td><td valign="top">Añadir la sección de Planes</td><td valign="top">2h</td><td valign="top">Camila</td><td valign="top">Done</td></tr>
<tr><td valign="top">C14</td><td valign="top">Responsive design subscription section</td><td valign="top">Añadir el respectivo responsive design para Planes</td><td valign="top">2h</td><td valign="top">Camila</td><td valign="top">Done</td></tr>
<tr><td rowspan="2" valign="top">US08 / EPIC01</td><td rowspan="2" valign="top">Implementación de un Footer</td><td valign="top">C15</td><td valign="top">Footer section</td><td valign="top"></td><td valign="top"></td><td valign="top">Andres</td><td valign="top"></td></tr>
<tr><td valign="top">C16</td><td valign="top">Responsive design footer section</td><td valign="top"></td><td valign="top"></td><td valign="top">Andres</td><td valign="top"></td></tr>
</table>

### 5.2.1.3 Development Evidence for Sprint Review

<table><tr><th valign="top"><b>Repository</b></th><th valign="top"><b>Branch</b></th><th valign="top"><b>Commit Id</b></th><th valign="top"><b>Commit Message</b></th><th valign="top"><b>Commit Message Body</b></th><th valign="top"><b>Committed on (Date)</b></th></tr>
<tr><td rowspan="10" valign="top">landing</td><td rowspan="10" valign="top">develop</td><td valign="top">f6d0bc6c84fde8f03f612d2c873897f62fe4000b</td><td valign="top">Initial commit</td><td valign="top"></td><td valign="top">9/04/2024</td></tr>
<tr><td valign="top">92c38ef84e51cc54f1716cc622579bede8b4f6ab</td><td valign="top">Update README.md</td><td valign="top"></td><td valign="top">9/04/2024</td></tr>
<tr><td valign="top">d85c4171401f63a4ba115f2b8dc1b6472187a3e1</td><td valign="top">feat: adding navbar & banner</td><td valign="top"></td><td valign="top">10/04/2024</td></tr>
<tr><td valign="top">3b9f05453e5c1f15ece59b07ef1ec5a6e8b4b910</td><td valign="top"><p>fix: adding logo & images</p><p></p></td><td valign="top"></td><td valign="top">11/04/2024</td></tr>
<tr><td valign="top">842b2a4f3080fd3149bfbd6dde5e242c4ea77205</td><td valign="top">fix: changing language to EN</td><td valign="top"></td><td valign="top">12/04/2024</td></tr>
<tr><td valign="top">cc50b26257ab0213f38ee474f0888d713291a887</td><td valign="top"><p>feat: add about us and features sections</p><p></p></td><td valign="top"></td><td valign="top">12/04/2024</td></tr>
<tr><td valign="top">37bacb7b604ef1f2b94c9a76945a448e0a195201</td><td valign="top"><p>feat: Contact us form added</p><p></p><p></p><p></p></td><td valign="top"></td><td valign="top">12/04/2024</td></tr>
<tr><td valign="top">8107fca1336b3e72ffbc497f63a759311998a79e</td><td valign="top">feat: add Mission and Vision, and Our Plans to index.html</td><td valign="top"></td><td valign="top">12/04/2024</td></tr>
<tr><td valign="top">014b64f5e077f05e8debd452b345a7ec9ca21b5b</td><td valign="top">feat: add respective style for Mission and Vision, and Our Plans styles.css</td><td valign="top"></td><td valign="top">13/04/2024</td></tr>
<tr><td valign="top">2b70b7d652a8b190bc7db02966c7d2770a9d1814</td><td valign="top">fix: correct the id for section Mission and Vision index.html</td><td valign="top"></td><td valign="top">14/04/2024</td></tr>
</table>

## 5.2.1.4 Testing Suite Evidence for Sprint Review
En esta parte del trabajo aún no se desarrolla el fronted, debido a eso no se pueden realizar Unit Test. Pero se agregaron nuevas user stories a las que ayudara mucho en el diseño de la pagina.

## 5.2.1.5 Execution Evidence for Sprint Review

- Se creó y configuró una barra de navegación para permitir la navegación fácil entre las diferentes secciones de la página

  ![image](/Assets/CHAPTER_V/inicio.png) 

- Se diseñó y desarrolló esta sección con un mensaje atractivo y convincente para los usuarios, y se implementó los botones "Comencemos" y "Saber mas"

  ![image](/Assets/CHAPTER_V/welcome.png)

- Se implemento la sección "Quienes Somos".

  ![image](/Assets/CHAPTER_V/somos.png)

- Se implemento la sección "Caracteristicas" para los usuarios.
  
  ![image](/Assets/CHAPTER_V/caracteristicas.png)

- Se completó la sección "Nuestros Proyectos" para que el usuario este enterado de nuestros en la landing page.

  ![image](/Assets/CHAPTER_V/nuestros_proyectos.png)

- Se añadio la seccion de "Unete" para que el usuario pueda ingresar sus datos

  ![image](/Assets/CHAPTER_V/unete.png)

- Se añadio la seccion de "Nuestros planes" para que el usuario pueda obserbar el plan profesional y el plan business

  ![image](/Assets/CHAPTER_V/planes.png)

## 5.2.1.6 Services Documentation Evidence for Sprint Review

Webstorm: Se optó por utilizar Webstorm como el Entorno Integrado de Desarrollo (IDE) principal para el desarrollo del landing page. Webstorm ofrece una amplia gama de características y funcionalidades que facilitan la escritura de código, la depuración y la gestión de proyectos.
HTML: Se hizo uso de HTML y Javacript, para dotar de interactividad y lógica a los diversos componentes del landing page.

GitHub:Se decidió alojar el repositorio del landing page en GitHub, una plataforma de desarrollo colaborativo basada en Git.

## 5.2.1.7 Software Deployment Evidence for Sprint Review

Se desplego la primera versión de nuestra LandingPage, donde mostramos lo que nuestros usuarios podrán ver dentro de nuestra aplicación web, si hay un bug o error presentando en esta landing será adecuadamente corregido en las proximas entregas.

## 5.2.1.8. Team Collaboration Insights during Sprint.
Se representan los commits y actividad del grupo durante el Sprint 1. En este caso, es sobre el avance de la Landing Page.

![](/Assets/InsightsSprint1A.png)
![](/Assets/InsightsSprint1B.png)

## 5.2.2. Sprint 2

#### 5.2.2.1 Sprint Planning 2

Se realizó una reunión en Meet con todos los integrantes del grupo presentes para poder asignar tareas a cada uno de estos. Asimismo, se creó un chat grupal en el WhatsApp para poder resolver las dudas que tengamos.

<table>
  <tr>
    <td align="center"><strong>Sprint #</strong></td>
    <td align="center"><strong>2</strong></td>
  </tr>
  <tr>
  <td colspan="2" align="center"><strong>Sprint Planning Background</strong></td>
  </tr>
  <tr>
    <td align="center">Date</td>
    <td align="center">2024/04/22</td>
  </tr>
  <tr>
    <td align="center">Time</td>
    <td align="center">12:00 PM</td>
  </tr>
  <tr>
    <td align="center">Location</td>
    <td align="center">Modalidad virtual, uso de Google Meets</td>
  </tr>
  <tr>
    <td align="center">Prepared By</td>
    <td align="center">Camila Cristina Loli Ramirez</td>
  </tr>
  <tr>
    <td align="center">Attendees (to planning meeting)</td>
    <td align="center">Alvaro Esteban Crispin Ccancce<br>Camila Cristina Loli Ramirez<br>Carlos Andres Rojas Ccama<br>Eduardo Renato Ventura Chancafe<br>Piero Mendoza Pimentel</td>
  </tr>
  <tr>
    <td align="center">Sprint 2 – 1 Review Summary</td>
    <td align="center">Se desplegó la Landing Page en Vercel y se empezó la planificación del Front-End de la aplicación. </td>
  </tr>
  <tr>
    <td align="center">Sprint 2 – 1 Retrospective Summary</td>
    <td align="center">Se planeó incluir la posibilidad de cambiar de idioma en la Landing Page. Inició el proceso de la creación del Front-End de BuildSphere. Priorizamos la creación de los componentes que definen a la aplicación (core).</td>
  </tr>
  <tr>
    <td colspan="2" align="center"><strong>Sprint Goal & User Stories</strong></td>
  </tr>
  <tr>
    <td align="center">Sprint 2 Goal</td>
    <td align="center">Se debe completar las vistas del Frontend en Webstorm y completar el Sprint 2</td>
  </tr>
  <tr>
    <td align="center">Sprint n Velocity</td>
    <td align="center">20</td>
  </tr>
  <tr>
    <td align="center">Sum of Story Points</td>
    <td align="center">20</td>
  </tr>
</table>

## 5.2.2.2 Sprint Backlog 2

<table>
  <tr>
    <td align="center"><strong>Sprint</td>
    <td colspan="7" align="center"><strong>1</strong></td>
  </tr>
  <tr>
    <td colspan="2" align="center"><strong>User Story</strong></td>
    <td colspan="6" align="center"><strong>Work-Item / Task</strong></td>
  </tr>
  <tr>
    <td align="center"><strong>ID</strong></td>
    <td align="center"><strong>Title</strong></td>
    <td align="center"><strong>ID</strong></td>
    <td align="center"><strong>Title</strong></td>
    <td align="center"><strong>Description</strong></td>
    <td align="center"><strong>Estimation (Hours)</strong></td>
    <td align="center"><strong>Assigned To</strong></td>
    <td align="center"><strong>Status (To-do / In-Process / To-Review / Done)</strong></td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI01</td>
    <td align="center">Perfil (Pequeña Empresa y Gran Empresa)</td>
    <td align="center">Crear las páginas de perfil para pequeña y gran empresa</td>
    <td align="center">6</td>
    <td align="center">Carlos Andres Rojas Ccama</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI02</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">4</td>
    <td align="center">-</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI03</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">4</td>
    <td align="center">-</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI04</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">4</td>
    <td align="center">-</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI05</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI06</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">7</td>
    <td align="center">-</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI07</td>
    <td align="center">Login (Pequeña Empresa y Gran Empresa)</td>
    <td align="center">Crear las páginas de login para pequeña y gran empresa</td>
    <td align="center">4</td>
    <td align="center">Carlos Andres Rojas Ccama</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI08</td>
    <td align="center">Registro (Pequeña Empresa y Gran Empresa)</td>
    <td align="center">Crear las páginas de registro para pequeña y gran empresa</td>
    <td align="center">4</td>
    <td align="center">Carlos Andres Rojas Ccama</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI09</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">6</td>
    <td align="center">-</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI09</td>
    <td align="center">Notificaciones</td>
    <td align="center">Crear las páginas de notificaciones</td>
    <td align="center">4</td>
    <td align="center">-</td>
    <td align="center">Done</td>
  </tr>
  <tr>
    <td align="center">No aplica</td>
    <td align="center">No aplica</td>
    <td align="center">WI09</td>
    <td align="center">Actualización del Informe</td>
    <td align="center"></td>
    <td align="center">5</td>
    <td align="center">Todo el grupo</td>
    <td align="center">Done</td>
  </tr>
</table>

## 5.2.2.3. Development Evidence for Sprint Review. 
<table>
  <tr>
    <td align="center"><strong>Repository</strong></td>
    <td align="center"><strong>Branch</strong></td>
    <td align="center"><strong>Commit ID</strong></td>
    <td align="center"><strong>Commit Message</strong></td>
    <td align="center"><strong>Commit Message Body</strong></td>
    <td align="center"><strong>Commited on (Date)</strong></td>
  </tr>
  <tr>
    <td align="center">https://github.com/ConstruTech-UPC/BuildSphere-front-end</td>
    <td align="center">feature/main</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">01/05/2024</td>
  </tr>
  <tr>
    <td align="center">https://github.com/ConstruTech-UPC/BuildSphere-front-end</td>
    <td align="center">feature/main</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">01/05/2024</td>
  </tr>
  <tr>
    <td align="center">https://github.com/ConstruTech-UPC/BuildSphere-front-end</td>
    <td align="center">feature/main</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">01/05/2024</td>
  </tr>
  <tr>
    <td align="center">https://github.com/ConstruTech-UPC/BuildSphere-front-end</td>
    <td align="center">feature/main</td>
    <td align="center">-</td>
    <td align="center">-</td>
    <td align="center">-</td>
  <td align="center">01/05/2024</td>
  <tr>
    <td align="center">https://github.com/ConstruTech-UPC/BuildSphere-front-end</td>
    <td align="center">Carlos Rojas</td>
    <td align="center">-</td>
    <td align="center">Add Login component & Udate Login</td>
    <td align="center">Add Login component & Udate Login</td>
  <td align="center">01/05/2024</td>
  <tr>
    <td align="center">https://github.com/ConstruTech-UPC/BuildSphere-front-end</td>
    <td align="center">Carlos Rojas</td>
    <td align="center">-</td>
    <td align="center">Merge pull request #15</td>
    <td align="center">Merge pull request #15</td>
  <td align="center">01/05/2024</td>
  
</table>

## 5.2.2.4. Testing Suite Evidence for Sprint Review. 

-

## 5.2.2.5. Execution Evidence for Sprint Review. 

Welcome

![imagen](/Assets/CHAPTER_V/bienvenido.png)

Login

![imagen](/Assets/CHAPTER_V/login.png)


Singup

![imagen](/Assets/CHAPTER_V/singup.png)


## 5.2.2.6. Services Documentation Evidence for Sprint Review. 

Para la creación de la plataforma,en esta caso para el desarrollo del Fronted se utilizo lo siguiente. 
*Webstorm (IDE DE DESARROLLO):* Hemos utilizado Webstorm como IDE para el desarrollo de nuestro Frontend. 

*Angular (Frameworks):* Usamos Angular como Frameworks de trabajo.

*GitHub:* Hemos alojado nuestro repositorio del Frontend en GitHub para colaborar y realizar un seguimiento más efectivo de los cambios en el código.

## 5.2.2.7. Software Deployment Evidence for Sprint Review. 

Para esta entrega se logró desplegar el front end de la aplicación en netlify. Link: 
https://66354ee2f6a8fe566da63fea--buildsphere.netlify.app/

## 5.2.2.8. Team Collaboration Insights during Sprint. 

![](/Assets/InsightsSprint2.png)

## 5.2.3. Sprint 3

#### 5.2.3.1 Sprint Planning 3
Se realizó una reunión en Meet con todos los integrantes del grupo para poder asignar tareas a cada uno de estos. Asimismo, se creó un chat grupal en el WhatsApp para poder resolver las dudas que tengamos.

<table>
  <tr>
    <td align="center"><strong>Sprint #</strong></td>
    <td align="center"><strong>3</strong></td>
  </tr>
  <tr>
  <td colspan="2" align="center"><strong>Sprint Planning Background</strong></td>
  </tr>
  <tr>
    <td align="center">Date</td>
    <td align="center">2024/05/13</td>
  </tr>
  <tr>
    <td align="center">Time</td>
    <td align="center">12:00 PM</td>
  </tr>
  <tr>
    <td align="center">Location</td>
    <td align="center">Modalidad virtual, uso de Google Meets</td>
  </tr>
  <tr>
    <td align="center">Prepared By</td>
    <td align="center">Camila Cristina Loli Ramirez</td>
  </tr>
  <tr>
    <td align="center">Attendees (to planning meeting)</td>
    <td align="center">Alvaro Esteban Crispin Ccancce<br>Camila Cristina Loli Ramirez<br>Carlos Andres Rojas Ccama<br>Eduardo Renato Ventura Chancafe<br>Piero Mendoza Pimentel</td>
  </tr>
  <tr>
    <td align="center">Sprint 3 – 2 - 1Review Summary</td>
    <td align="center">Se desplegó la Landing Page en Vercel y se empezó la planificación del Front-End de la aplicación. </td>
  </tr>
  <tr>
    <td align="center">Sprint 3 - 2 – 1 Retrospective Summary</td>
    <td align="center">Se planeó incluir la posibilidad de cambiar de idioma en la Landing Page. Arreglar mínimos detalles en el front-end. Asimismo, empezó el desarrollo del back-end de la aplicación en java, se priorizó el core de la empresa (project, documents, resource, operations management).</td>
  </tr>
  <tr>
    <td colspan="2" align="center"><strong>Sprint Goal & User Stories</strong></td>
  </tr>
  <tr>
    <td align="center">Sprint 3 Goal</td>
    <td align="center"> Se debe realizar correcciones para Front-End para la implementación del Backend. Empezar el desarrollo del backend y que los endpoints respectivos funcionen, sean visibles en Swagger.</td>
  </tr>
  <tr>
    <td align="center">Sprint n Velocity</td>
    <td align="center">2 semanas</td>
  </tr>
  <tr>
    <td align="center">Sum of Story Points</td>
    <td align="center">20</td>
  </tr>
</table>

#### 5.2.3.2.Sprint Backlog 3

<table>
<tr><th colspan="2" valign="top">Sprint #</th><th colspan="6" valign="top">Sprint 3</th></tr>
<tr><td colspan="2" valign="top">User story</td><td colspan="6" valign="top">Work Item/ Task</td></tr>
<tr><td valign="top"><b>Id</b></td><td valign="top"><b>Title</b></td><td valign="top"><b>Id</b></td><td valign="top"><b>Title</b></td><td valign="top"><b>Description</b></td><td valign="top"><b>Estimation(hours)</b></td><td valign="top"><b>Assigned to</b></td><td valign="top"><b>Status(To-do /InProcess To Review Done)</b></td></tr>

<tr>
    <td rowspan="2" valign="top">TS01</td>
    <td rowspan="2" valign="top">Añadir un perfil con el uso del RESTful API</td>
    <td valign="top">C01</td>
    <td valign="top">Crear endpoint para la creacion de un perfil</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Eduardo</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS02</td>
    <td rowspan="2" valign="top">Visualizar un perfil con el uso del RESTful API</td>
    <td valign="top">C02</td>
    <td valign="top">Crear endpoint para la vizualizacion de un perfil</td>
    <td valign="top">Implementación de un método GET para la obtencion de datos</td>
    <td valign="top">3</td>
    <td valign="top">Eduardo</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS03</td>
    <td rowspan="2" valign="top">Añadir un proyecto con el uso del RESTful API</td>
    <td valign="top">C03</td>
    <td valign="top">Crear endpoint para la creacion de un proyecto</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Eduardo</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS04</td>
    <td rowspan="2" valign="top">Editar un proyecto con el uso del RESTful API</td>
    <td valign="top">C04</td>
    <td valign="top">Crear endpoint para la edicion de un proyecto</td>
    <td valign="top">Implementación de un método PUT para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Eduardo</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS05</td>
    <td rowspan="2" valign="top">Eliminar un proyecto con el uso del RESTful API</td>
    <td valign="top">C05</td>
    <td valign="top">Crear endpoint para la eliminacion de un proyecto</td>
    <td valign="top">Implementación de un método DELETE para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Eduardo</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS06</td>
    <td rowspan="2" valign="top">Vizualizar un proyecto con el uso del RESTful API</td>
    <td valign="top">C06</td>
    <td valign="top">Crear endpoint para la visualizacion de un proyecto</td>
    <td valign="top">Implementación de un método GET para la obtencion ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Eduardo</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS07</td>
    <td rowspan="2" valign="top">Añadir un documento con el uso del RESTful API</td>
    <td valign="top">C07</td>
    <td valign="top">Crear endpoint para la cracion de un documento</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Alvaro</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS08</td>
    <td rowspan="2" valign="top">Editar un documento con el uso del RESTful API</td>
    <td valign="top">C08</td>
    <td valign="top">Crear endpoint para la edicion de un documento</td>
    <td valign="top">Implementación de un método PUT para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Alvaro</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS09</td>
    <td rowspan="2" valign="top">Eliminar un documento con el uso del RESTful API</td>
    <td valign="top">C09</td>
    <td valign="top">Crear endpoint para la eliminacion de un documento</td>
    <td valign="top">Implementación de un método DELETE para la eliminacion de datos</td>
    <td valign="top">3</td>
    <td valign="top">Alvaro</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
<tr>
    <td rowspan="2" valign="top">TS10</td>
    <td rowspan="2" valign="top">Añadir material con el uso del RESTful API</td>
    <td valign="top">C10</td>
    <td valign="top">Crear endpoint para el ingreso de materiales</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
</tr>
<tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS11</td>
    <td rowspan="2" valign="top">Editar un material con el uso del RESTful API</td>
    <td valign="top">C11</td>
    <td valign="top">Crear endpoint para la edición de un material</td>
    <td valign="top">Implementación de un método PUT para la edición de datos</td>
    <td valign="top">2</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
  </tr>
<tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS12</td>
    <td rowspan="2" valign="top">Eliminar un material con el uso del RESTful API</td>
    <td valign="top">C12</td>
    <td valign="top">Crear endpoint para la eliminación de un material</td>
    <td valign="top">Implementación de un método DELETE para eliminar el material</td>
    <td valign="top">1</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
  </tr>
<tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS13</td>
    <td rowspan="2" valign="top">Añadir una máquina con el uso del RESTful API</td>
    <td valign="top">C13</td>
    <td valign="top">Crear endpoint para el ingreso de máquinas</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">3</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
  </tr>
<tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS14</td>
    <td rowspan="2" valign="top">Editar una máquina con el uso del RESTful API</td>
    <td valign="top">C14</td>
    <td valign="top">Crear endpoint para la edición de una máquina</td>
    <td valign="top">Implementación de un método PUT para la edición de datos</td>
    <td valign="top">2</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
  </tr>
<tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS15</td>
    <td rowspan="2" valign="top">Eliminar una máquina con el uso del RESTful API</td>
    <td valign="top">C15</td>
    <td valign="top">Crear endpoint para la eliminación de una máquina</td>
    <td valign="top">Implementación de un método DELETE para eliminar la máquina</td>
    <td valign="top">1</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
  </tr>
<tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS16</td>
    <td rowspan="2" valign="top">Visualizar toda la maquinaria disponible en un proyecto</td>
    <td valign="top">C16</td>
    <td valign="top">Crear endpoint para la visualización de máquinas dentro de un proyecto</td>
    <td valign="top">Implementación de un método GET para mostrar todas las máquinas</td>
    <td valign="top">1</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
  </tr>
<tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS17</td>
    <td rowspan="2" valign="top">Visualizar todos los materiales disponibles en un proyecto</td>
    <td valign="top">C17</td>
    <td valign="top">Crear endpoint para la visualización de materiales dentro de un proyecto</td>
    <td valign="top">Implementación de un método GET para mostrar todos los materiales</td>
    <td valign="top">1</td>
    <td valign="top">Camila</td>
    <td valign="top">Done</td>
  </tr>
  <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS18</td>
    <td rowspan="2" valign="top">Añadir un equipo con el uso del RESTful API</td>
    <td valign="top">C18</td>
    <td valign="top">Crear endpoint para el ingreso de un equipo</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
    <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS19</td>
    <td rowspan="2" valign="top">Editar un equipo con el uso del RESTful API</td>
    <td valign="top">C19</td>
    <td valign="top">Crear endpoint para la edicion de un equipo</td>
    <td valign="top">Implementación de un método PUT para la edición de datos</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
      <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS20</td>
    <td rowspan="2" valign="top">Eliminar un equipo con el uso del RESTful API</td>
    <td valign="top">C20</td>
    <td valign="top">Crear endpoint para la eliminacion de un equipo</td>
    <td valign="top">Implementación de un método DELETE para eliminar un equipo</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
      <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS21</td>
    <td rowspan="2" valign="top">Visualizar todos los equipos con disponibles en un proyecto</td>
    <td valign="top">C21</td>
    <td valign="top">Crear endpoint para la visualizacion de equipos de un proyecto</td>
    <td valign="top">Implementación de un método GET para mostrar todos los equipos</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
  <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS22</td>
    <td rowspan="2" valign="top">Añadir un trabajador con el uso del RESTful API</td>
    <td valign="top">C22</td>
    <td valign="top">Crear endpoint para el ingreso de un trabajador</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
    <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS23</td>
    <td rowspan="2" valign="top">Editar un trabajador con el uso del RESTful API</td>
    <td valign="top">C19</td>
    <td valign="top">Crear endpoint para la edicion de un trabajador</td>
    <td valign="top">Implementación de un método PUT para la edición de datos</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
      <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS24</td>
    <td rowspan="2" valign="top">Eliminar un trabajador con el uso del RESTful API</td>
    <td valign="top">C24</td>
    <td valign="top">Crear endpoint para la eliminacion de un trabajador</td>
    <td valign="top">Implementación de un método DELETE para eliminar un trabajador</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
      <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS25</td>
    <td rowspan="2" valign="top">Visualizar todos los trabajadores disponibles en un proyecto</td>
    <td valign="top">C25</td>
    <td valign="top">Crear endpoint para la visualizacion de trabajadores de un proyecto</td>
    <td valign="top">Implementación de un método GET para mostrar todos los trabajadores</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">Done</td>
  </tr>
  <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS26</td>
    <td rowspan="2" valign="top">Añadir una tarea con el uso del RESTful API</td>
    <td valign="top">C26</td>
    <td valign="top">Crear endpoint para el ingreso de una tarea</td>
    <td valign="top">Implementación de un método POST para el ingreso de datos</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">To do</td>
  </tr>
    <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS27</td>
    <td rowspan="2" valign="top">Editar una tarea con el uso del RESTful API</td>
    <td valign="top">C27</td>
    <td valign="top">Crear endpoint para la edición de una tarea</td>
    <td valign="top">Implementación de un método PUT para la edición de datos</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">To do</td>
  </tr>
      <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS28</td>
    <td rowspan="2" valign="top">Eliminar una tarea con el uso del RESTful API</td>
    <td valign="top">C28</td>
    <td valign="top">Crear endpoint para la eliminación de una tarea</td>
    <td valign="top">Implementación de un método DELETE para eliminar una tarea</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">To do</td>
  </tr>
      <tr></tr>
  <tr>
    <td rowspan="2" valign="top">TS29</td>
    <td rowspan="2" valign="top">Visualizar todas las tareas disponibles en un proyecto</td>
    <td valign="top">C29</td>
    <td valign="top">Crear endpoint para la visualización de tareas de un proyecto</td>
    <td valign="top">Implementación de un método GET para mostrar todos las tareas</td>
    <td valign="top">2</td>
    <td valign="top">Piero</td>
    <td valign="top">To do</td>
  </tr>
  </table>


#### 5.2.3.3.Development Evidence for Sprint Review

<table>
  <tr>
    <td align="center"><strong>Repository</strong></td>
    <td align="center"><strong>Branch</strong></td>
    <td align="center"><strong>Commit ID</strong></td>
    <td align="center"><strong>Commit Message</strong></td>
    <td align="center"><strong>Commit Message Body</strong></td>
    <td align="center"><strong>Commited on (Date)</strong></td>
  </tr>
    <tr>
    <td align="center">https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">55a3a36c1469ad066bf368640e90869d152a2c57</td>
    <td align="center">initial commit</td>
    <td align="center">-</td>
    <td align="center">May 25, 2024</td>
  </tr>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">889001ab4dbe0c08f74b5d2649baa09e06adb33f</td>
    <td align="center">chore: added auditable base types</td>
    <td align="center">-</td>
    <td align="center">May 28, 2024</td>
  </tr>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">056d58f7d95bc8449cc6fcd0b510e8e3f6913db0</td>
    <td align="center">Create OpenApiConfiguration.java</td>
    <td align="center">-</td>
    <td align="center">01/06/2024</td>
  </tr>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">4f761713d6b0e77e183caa5d737b23bdfa290019</td>
    <td align="center">feat: valueObjects created</td>
    <td align="center">-</td>
    <td align="center">Jun 1, 2024</td>
  </tr>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">556259d4918c9d98f3014af7e59932aea79eda6c</td>
    <td align="center">feat: document aggregate created</td>
    <td align="center">-</td>
    <td align="center">Jun 1, 2024</td>
  </tr>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">4792b47b6105674ef6ac2118ea717ac3ba33246b</td>
    <td align="center">feat: shared abstract models created</td>
    <td align="center">-</td>
  <td align="center">01/06/2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">7b98e51633794d48c18f4ee1f3188d4d4c4c7beb</td>
    <td align="center">feat(shared-context): Implement Shared Bounded Context</td>
    <td align="center">-</td>
  <td align="center">Jun 5, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">7b98e51633794d48c18f4ee1f3188d4d4c4c7beb</td>
    <td align="center">feat(shared-context): Implement Shared Bounded Context</td>
    <td align="center">-</td>
  <td align="center">Jun 5, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">556259d4918c9d98f3014af7e59932aea79eda6c</td>
    <td align="center">feat: document aggregate created</td>
    <td align="center">-</td>
  <td align="center">Jun 1, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">899dcff6dae5be339cdff6b9bd5d52f704953f34</td>
    <td align="center">feat: adding commands to documents</td>
    <td align="center">-</td>
  <td align="center">Jun 5, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">899dcff6dae5be339cdff6b9bd5d52f704953f34</td>
    <td align="center">feat: creating query to get documents</td>
    <td align="center">-</td>
  <td align="center">Jun 5, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">e7b11e7bee01fd5c54aaf650684aa4d4a7e33c28</td>
    <td align="center">add: teams class in aggregates</td>
    <td align="center">-</td>
  <td align="center">Jun 6, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">69fa0d75d4fc0665129d5d17445886efea6c67f3</td>
    <td align="center">feat(teams): added commands, queries and value objects in domain</td>
    <td align="center">-</td>
  <td align="center">Jun 6, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">537e1ff3f8107c299c0de96b5b99aacd8da7ea35</td>
    <td align="center">feat(teams): added service contracts in domain</td>
    <td align="center">-</td>
  <td align="center">Jun 6, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">6d490a3b818e6a614cbf0144ae02fe44a612cb15</td>
    <td align="center">feat(teams): added controller service for team</td>
    <td align="center">-</td>
  <td align="center">Jun 6, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">b61936a6ca59eb02d4f2348560072cc253643879</td>
    <td align="center">feat: document repository</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">70d3131f861954f2e2a4f2c7a59b95077c5c2195</td>
    <td align="center">feat: add new document resource</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">644f774fa27301593feaf9a9ba3662b3207bea25</td>
    <td align="center">feat: document controller</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">6a398cc6fcd6613d329023de89d28bfc9013ad0d</td>
    <td align="center">add: worker class in aggregates</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">f6e365f14e5508346f15a5b47092caf59a11a82c</td>
    <td align="center">feat(workers): added service contracts in domain</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">f576b8e2d90dc590cfa3d4c39e35f9b0fc789f4f</td>
    <td align="center">feat(workers): added command and query services implementation</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">a2b35d70e291a0eb197b6f363a7567ce426d7481</td>
    <td align="center">feat(workers): added resources and assemblers for interfaces layer.</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">0553302735b9dda848864c1925317d54d6513d23</td>
    <td align="center">feat(workers): added controller service for worker.</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">57ec8d2b9a9792d9b92b657046a8b5e958560456</td>
    <td align="center">feat: swagger ui configuration</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">6cc5d4799e1450bab85ed5e440d76e538310a107</td>
    <td align="center">feat: update document command</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">e3fdb9eb05051b74ba50d143da7e1d1597824739</td>
    <td align="center">feat: added value objects for the aggregates.</td>
    <td align="center">-</td>
  <td align="center">Jun 7, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">c2d1c7c1ecd57f91b02291af82dcc701db15e047</td>
    <td align="center">feat: added aggregate for machine.</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">769393a3d1d5b304f0da6e7d5fbe8b4c28c9c4bd</td>
    <td align="center">feat: added aggregate for Material.</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">ad4f7b2b6a586838d347b11a704d1eb3ede9ffd1</td>
    <td align="center">feat: added command for create material.</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">695d31be10191320b3919aca073264659cf2cb96</td>
    <td align="center">feat: added create command in aggregate for Material.</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">5d6cd16a1e6fe5324311d67e315ff0e1c92a37f9</td>
    <td align="center">feat(project_management): add domain layer with aggregates, entities, value objects, commands, and queries</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">42d86485569df47410c475ee7441ccae682f67d2</td>
    <td align="center">feat: added command services for both aggregates.</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">ed8c353c7a9c2a2d6677ae6210f3d5e7efef2bba</td>
    <td align="center">feat(project_management): add services to domain layer</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">6b87cebf8cd3da875de66d89ae6e5c71ba063b34</td>
    <td align="center">feat(project_management): add and fix infrastructure and interfaces layers</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">364a15539824c5b26757289c9ad726d82aa318bb</td>
    <td align="center">feat(controller): implemented document controller</td>
    <td align="center">-</td>
  <td align="center">Jun 8, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">bc11713f0198734dd4e77db847759921154135b0</td>
    <td align="center">docs: initial configuration for swagger</td>
    <td align="center">-</td>
  <td align="center">Jun 9, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">a35f26f60a3ef4f76cccf0440e2894fb1bbdccce</td>
    <td align="center">feat: added the resources for material and machine (create, update).</td>
    <td align="center">-</td>
  <td align="center">Jun 9, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">cc82a4e63c2493f40699e23f09499bde5f9123b1</td>
    <td align="center">Merge branch 'refs/heads/DocumentManagement' into development</td>
    <td align="center">-</td>
  <td align="center">Jun 9, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">ec7b886b4bf99d7c3b600f4c2382787ba5f501e6</td>
    <td align="center">Merge remote-tracking branch 'refs/remotes/origin/featureIAM' into development</td>
    <td align="center">-</td>
  <td align="center">Jun 9, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">6e4a9abdb6cf3ae182dc9551a332a8c7dd93b291</td>
    <td align="center">Merge remote-tracking branch 'refs/remotes/origin/feature/project-management' into development</td>
    <td align="center">-</td>
  <td align="center">Jun 9, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">78d8e3c8cee7dff60cde6de8aa2b822aa2f48bc7</td>
    <td align="center">Merge remote-tracking branch 'refs/remotes/origin/featureInventoryManagement' into development</td>
    <td align="center">-</td>
  <td align="center">Jun 9, 2024</td>
  <tr>
    <td align="center"> https://github.com/ConstruTech-UPC/back-end</td>
    <td align="center">feature/main</td>
    <td align="center">873a2ef1fb4947d6f5c2b20b7cb0e0ed09a01b9a</td>
    <td align="center">Merge remote-tracking branch 'refs/remotes/origin/featureOperationsManagement' into development</td>
    <td align="center">-</td>
  <td align="center">Jun 9, 2024</td>
</table>

#### 5.2.3.4.Testing Suite Evidence for Sprint Review
Para este sprint no se contempló la realización funcionalidades referente al testing de los endpoints de nuestra API, por lo que la tabla se mostrará vacía

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Committed on (Date)|
| :- | :- | :- | :- | :- | :- |
|||||||

Sin embargo, la comprobación de los endpoints se realizó mediante la herramienta de Swagger:

![Endpoints for Resources](/Assets/TestingSuite/EndPointsResources.png)


#### 5.2.3.5.Execution Evidence for Sprint Review

Para esta entrega se ha logrado implementar y desplegar la segunda version del Landing Page, la tercera versión del Frontend y primera version del backend.

## Landing Page

#### About the product

  ![image](/Assets/CHAPTER_V/Imagenes%20landing%20page/About%20the%20product.PNG)

#### About the team

  ![image](/Assets/CHAPTER_V/Imagenes%20landing%20page/About%20the%20team.PNG)

#### Contact us

  ![image](/Assets/CHAPTER_V/Imagenes%20landing%20page/Contact%20us.PNG)

#### Mision and vision

  ![image](/Assets/CHAPTER_V/Imagenes%20landing%20page/Mision%20y%20vision.PNG)

#### Plans

  ![image](/Assets/CHAPTER_V/Imagenes%20landing%20page/Plans.PNG)

Video Frontend: https://upcedupe-my.sharepoint.com/:v:/g/personal/u201923446_upc_edu_pe/Eem7n63KrxdCpawOCQCPpvYB9R-8UDYEfh6GRNW3Jk5cOg?e=OL1162&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

## Frontend

#### Projects

  ![image](/Assets/Execution%20Evidence%20for%20Sprint%20Review/Projectos.png)

#### Resource Management

![image](/Assets/Execution%20Evidence%20for%20Sprint%20Review/Inventory%20Mangement.png)

#### Collaboration

![image](/Assets/Execution%20Evidence%20for%20Sprint%20Review/Collaboration%20worker%20team.png)

#### Documents

![image](/Assets/Execution%20Evidence%20for%20Sprint%20Review/Documents.png)

Video Frontend: https://upcedupe-my.sharepoint.com/:v:/g/personal/u201923446_upc_edu_pe/ET5KaWG1dbtOpdmiPzyv5kkB0kLo-FHq8e3om0j2GfWUww?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=33JY0B

## Backend

#### Materials

![image](/Assets/CHAPTER_V/Imagenes%20backend/Materials.jpeg)

#### Teams and Profiles

![image](/Assets/CHAPTER_V/Imagenes%20backend/Team%20and%20profiles.jpeg)

#### Machines and Documents

![image](/Assets/CHAPTER_V/Imagenes%20backend/Machines%20and%20documents.jpeg)

#### Projects and Workers
![image](/Assets/CHAPTER_V/Imagenes%20backend/Projects%20and%20workers.jpeg)

Video Backend: https://upcedupe-my.sharepoint.com/:v:/g/personal/u201923446_upc_edu_pe/EWih8CavWH5Kigv-uw6ZpIkBL7hCl45cHnpAfmiW7LtUQQ?e=ayphtP&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

#### 5.2.3.6.Services Documentation Evidence for Sprint Review

En esta sección se presentan los endpoints desarrollados durante el sprint y se adjuntan capturas de la UI de swagger con OpenApi. En el alcance de este sprint se han desarrollado los bounded context de authentication, resource management, operations, document and projects.
Se adjunta el enlace al repositorio correspondiente: https://github.com/ConstruTech-UPC/back-end.git  
Se adjunta el enlace del back end desplegado: https://construtech-production.up.railway.app/swagger-ui/index.html#/

||||
| :- | :- | :- |
|Entity|EndPoint URL|Swagger|
|Document|/api/v1/documents|![image](/Assets/CHAPTER_V/endpoints/Aspose.Words.52aed607-83ba-41ac-8660-2b8fc985849e.001.png)|
|Material|/api/v1/materials|![image](/Assets/CHAPTER_V/endpoints/Aspose.Words.52aed607-83ba-41ac-8660-2b8fc985849e.002.jpeg)|
|Machine|/api/v1/machines|![image](/Assets/CHAPTER_V/endpoints/Aspose.Words.52aed607-83ba-41ac-8660-2b8fc985849e.003.jpeg)|
|Profile|/api/v1/profiles|![image](/Assets/CHAPTER_V/endpoints/Aspose.Words.52aed607-83ba-41ac-8660-2b8fc985849e.004.png)|
|Project|/api/v1/projects|![image](/Assets/CHAPTER_V/endpoints/Aspose.Words.52aed607-83ba-41ac-8660-2b8fc985849e.005.png)|
|Team|/api/v1/teams|![image](/Assets/CHAPTER_V/endpoints/Aspose.Words.52aed607-83ba-41ac-8660-2b8fc985849e.006.png)|
|Worker|/api/v1/workers|![image](/Assets/CHAPTER_V/endpoints/Aspose.Words.52aed607-83ba-41ac-8660-2b8fc985849e.007.png)|

#### 5.2.3.7.Software Deployment Evidence for Sprint Review

Primero, accedemos a railway.com e iniciamos sesión. Luego, navegamos hasta la sección donde haremos clic en "Start a New Project".

![image](/Assets/CHAPTER_V/railway%20inicio.png)

Luego, en la siguiente pantalla, seleccionamos la opción "Deploy MySQL".

![image](/Assets/CHAPTER_V/deploysql.png)

En la siguiente sección, aparecerán varias opciones de configuración para nuestro archivo appsettings.json, las cuales necesitaremos actualizar.

![image](/Assets/CHAPTER_V/sqlSettings.png)

Tras haber hecho eso solo presionaremos en Deploy y se desplegará la base de datos y la lógica de backend en 2 servicios que estarán interconectados.

![image](/Assets/CHAPTER_V/sqldesplegado.png)

Es importante destacar que, al llegar a este punto, obtendremos un dominio público que nos permitirá realizar consultas a través de Postman e interactuar con nuestra base de datos.

**Link de la base de datos desplegada:** https://construtech-production.up.railway.app/


#### 5.2.3.8.Team Collaboration Insights during Sprint 

![image](/Assets/InsightsSprint3.png)

#### 5.2.4.2. Sprint Backlog 4.


|<p># Orden </p><p></p>|User Story Id|Título |Descripción |<p>Story Points (1 / 2 / 3 / 5</p><p>/ 8)</p>|
| :- | :- | :- | :- | :- |
|1|US-24|Como usuario deseo poder agregar, editar y eliminar maquinarias dentro de un proyecto|El usuario desea tener un control de todos las maquinarias que hay dentro de un proyecto para tener un mejor control de sus recursos|3|
|2|US-25|Como usuario deseo poder agregar, editar y eliminar materiales dentro de un proyecto|El usuario desea tener un control de todos los materiales que hay dentro de un proyecto para tener un mejor control de sus recursos|3|
|3|US-26|Como usuario deseo poder agregar, editar y eliminar documentos dentro de un proyecto|El usuario desea tener un control de todos los documentos que hay dentro de un proyecto para tener un mejor control de sus recursos|3|
|4|US-27|Como usuario deseo poder agregar, editar y eliminar documentos dentro de un proyecto|El usuario desea tener un control de todos los documentos que hay dentro de un proyecto para tener un mejor control de sus recursos|2|
|5|US-28|Como usuario deseo poder agregar, editar y eliminar trabajadores dentro de un proyecto|El usuario desea tener un control de todos los trabajadores que hay dentro de un proyecto para tener un mejor control de sus recursos|3|
|6|US-29|Como usuario deseo poder agregar, editar y eliminar equipos de trabajo dentro de un proyecto|El usuario desea tener un control de todos los trabajadores que hay dentro de un proyecto para tener un mejor control de sus recursos|3|
|7|US-30|Como usuario deseo poder agregar, editar y eliminar tareas de trabajo dentro de un proyecto|El usuario desea tener un control de todos las tareas que hay dentro de un proyecto para tener un mejor control de sus recursos|3|
|8|US-30|Como usuario deseo poder agregar, editar y eliminar mis datos de trabajo dentro de un proyecto|<p>El usuario desea tener un control de todos sus datos</p><p>que hay dentro de un proyecto para tener un mejor control</p><p>de sus recursos</p><p></p>|3|
|9|US-31|Como usuario deseo poder agregar, editar y eliminar roles de trabajo dentro de un proyecto|<p>El usuario desea tener un control de todos los roles</p><p>que hay dentro de un proyecto para tener un mejor control</p><p>de sus recursos</p><p></p>|3|
|8|TS-X|Autenticación del usuario|Crear un endpoint con método POST para permitir el ingreso del usuario|2|
|9|TS-X|Gestión de sesiones|Creación de un token para cada usuario al momento de iniciar sesión y que cuente con una fecha de expiración|3|
|10|TS-X|Auditoría de sesiones|Registra la fecha y hora de la creación para los features (cuando se creó un documento, un equipo, un material, un proyecto, etc.) disponibles.|2|

#### 5.2.4.3. Development Evidence for Sprint Review.

Enlace del repositorio trabajado durante el sprint: <https://github.com/ConstruTech-UPC/back-end.git> 

<table><tr><th valign="top">Repository</th><th valign="top">Branch</th><th valign="top">Commit Id</th><th valign="top">Commit Message</th><th valign="top">Commit Message Body</th><th valign="top">Committed on (Date)</th></tr>
<tr><td rowspan="5" valign="top">ConstruTech-UPC/back-end</td><td valign="top">featureIAM</td><td valign="top">635f6bd</td><td valign="top">feat(iam): added role and user</td><td valign="top"></td><td valign="top">10/06/2024</td></tr>
<tr><td valign="top">feature/project-management</td><td valign="top">6b87ceb</td><td valign="top">feat(project_management): add and fix infrastructure and interfaces layers</td><td valign="top"></td><td valign="top">09/06/2024</td></tr>
<tr><td valign="top">featureInventoryManagement</td><td valign="top">5d86d41</td><td valign="top">feat: added controllers for Machine and Material (includes delete, create, delete)</td><td valign="top"></td><td valign="top">07/06/2024</td></tr>
<tr><td valign="top">featureOperationManagement</td><td valign="top">0553302</td><td valign="top"><p>feat(workers): added controller service for worker</p><p></p></td><td valign="top"></td><td valign="top">07/06/2024</td></tr>
<tr><td valign="top">development</td><td valign="top">873a2ef</td><td valign="top">Merge remote-tracking branch 'refs/remotes/origin/featureOperationsManagement</td><td valign="top"></td><td valign="top">11/06/2024</td></tr>
</table>




#### 5.2.4.4. Testing Suite Evidence for Sprint Review.

Para este sprint no se contempló la realización funcionalidades referente al testing de los endpoints de nuestra API, por lo que la tabla se mostrará vacía

|Repository|Branch|Commit Id|Commit Message|Commit Message Body|Committed on (Date)|
| :- | :- | :- | :- | :- | :- |
|https://github.com/ConstruTech-UPC/back-end/| main | 831621b | feat(test): added deleteMaterialSuccessful to test if it works. | |26/06/2024|

#### 5.2.4.5. Execution Evidence for Sprint Review.

Se mostrarán las capturas necesarias de la aplicación que se llevaron a cado durante este sprint



#### 5.2.4.6. Services Documentation Evidence for Sprint Review.

En esta sección se presentan los endpoints desarrollados durante el sprint y se adjuntan capturas de la UI de swagger con OpenApi. En el alcance de este sprint se han desarrollado los bounded context de authentication, resource management, operations, document and projects.

Se adjunta el enlace al repositorio correspondiente: <https://github.com/ConstruTech-UPC/back-end.git>  

|Bounded Context|Documentation||
| :- | :- | :- |
|Entity|EndPoint URL|Swagger|
|Document|/api/v1/documents|![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.001.png)|
|Material|/api/v1/materials|![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.002.jpeg)|
|Machine|/api/v1/machines|![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.003.jpeg)|
|Profile|/api/v1/profiles|![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.004.png)|
|Project|/api/v1/projects|![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.005.png)|
|Team|/api/v1/teams|![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.006.png)|
|Worker|/api/v1/workers|![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.007.png)|

#### 5.2.3.7. Software Deployment Evidence for Sprint Review.

De la misma forma que se hizo en los anteriores sprints se continúa usando el servicio de despliegue Vercel. 

#### 5.2.3.8. Team Collaboration Insights during Sprint.

Para este sprint como se mencionó se mejoraron las vistas en todas las pestañas del front-end. A continuación se presentará los insights del grupo.

Enlace del repositorio: <https://github.com/ConstruTech-UPC/BuildSphere-front-end> 

![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.008.png)

Así mismo, presentamos las ramas que se desarrollaron para la implementación de los features

![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.009.png)

Enlace al back-end: <https://github.com/ConstruTech-UPC/back-end> 

Para el desarrollo del RESTFulAPI, se han implementado los endpoints según el bounded context del negocio

![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.010.png)

De la misma manera, se presenta el gráfico con las ramas que se desarrollaron para los endpoints

![image](/Assets/CHAPTER_V/Sprint4/Aspose.Words.a2dbc74c-d5b3-4ff0-9fa8-4bc46655b1cf.011.png)



## 5.3. Validation Interviews

### 5.3.1. Diseño de Entrevistas 

## Contratistas independientes y pequeñas empresas constructoras

### Preguntas Introductorias:

- ¿Cuál es su nombre?
- ¿Cuántos años tiene?
- ¿Cuáles son sus hobbies?
- ¿Qué ocupación tiene y cuál es el tamaño de su empresa?
- ¿Cuánto tiempo lleva trabajando en la industria de la construcción?
- ¿Cuál es su rol específico dentro de su empresa?

### Landing Page
- ¿Qué le parece la apariencia general de nuestra página de inicio?
- ¿La información presentada sobre las funcionalidades de la aplicación es clara y relevante para sus necesidades?
- ¿Qué cambiaría o añadiría para mejorar la presentación de la página de inicio
- ¿Hay algún aspecto de la navegación o diseño que encuentre confuso?

### Aplicación web
- ¿Qué opina del diseño y la disposición de la aplicación web?
- ¿Le resulta fácil entender y navegar por las distintas secciones de la aplicación?
- ¿Qué le parece la forma en que se muestran los proyectos?
- ¿El diseño de la lista o el formulario de creación de proyectos es intuitivo? ¿Qué mejoraría?
- ¿Qué opina sobre la disposición y gestión de los trabajadores, equipos y tareas?
- ¿Qué le parece la visualización del inventario de maquinaria y materiales?
- ¿Hay alguna funcionalidad adicional que le gustaría ver en la aplicación para facilitar su trabajo como contratista o pequeña empresa?
- ¿Considera que esta aplicación mejoraría su gestión de proyectos de construcción?
- ¿Estaría dispuesto a utilizar esta aplicación en sus proyectos actuales o futuros? ¿Por qué?
- ¿Qué valor agregado cree que esta aplicación podría ofrecer a su negocio?

## Grandes empresas de construccion

### Información personal
- ¿Cuál es su nombre completo?
- ¿Cuántos años tiene?
- ¿En qué distrito reside?
- ¿Qué ocupación tiene y cuál es el tamaño de su empresa?
- ¿Cuánto tiempo lleva trabajando en su lugar de oficio?
- ¿Cuál es su rol específico dentro de su empresa?
- A fin de recordar un poco la entrevista pasada, para tener en cuenta la validación, ¿qué sistema operativo utiliza mayormente (windows, linux, macOS), navegador (firefox, google chrome, safari), y dispositivo (celular, computadora, laptop)?

### Landing Page
- ¿Qué le parece la apariencia general de nuestra página de inicio?
- ¿La información presentada sobre las funcionalidades de la aplicación es clara y relevante para sus necesidades?
- ¿Qué cambiaría o añadiría para mejorar la presentación de la página de inicio?
- ¿Encontró fácil la navegación por la página de inicio?
- ¿Pudo encontrar rápidamente la información que estaba buscando?
- ¿Hay algún aspecto de la navegación o diseño que encuentre confuso?
Luego de revisar la página, ¿entiende claramente lo que hace BuildSphere?
- ¿Hay información adicional que le gustaría ver en la página de inicio?
- A su parecer, ¿el diseño le parece profesional?
- ¿Encontró alguna dificultad al usar la página de inicio?
- ¿Cuál fue su primera impresión respecto a la página?

### Aplicación web
- ¿Qué opina del diseño y la disposición de la aplicación web?
- ¿Le resulta fácil entender y navegar por las distintas secciones de la aplicación?
- ¿Qué tan fácil le fue interactuar con los elementos de la aplicación?
- ¿Experimentó alguna frustración al momento de usarlo?
- ¿Qué tan intuitivos son los controles y las interacciones de la aplicación?
- ¿Qué le parece la forma en que se muestran los proyectos?
- ¿El diseño de la lista o el formulario de creación de proyectos es intuitivo? ¿Qué mejoraría?
- ¿Considera que la opción de crear más de tres proyectos es útil? *Esto es en referencia que el segmento anterior no tiene opción de más proyectos debido a que es otro tipo de plan.
- ¿Qué opina sobre la disposición y gestión de los trabajadores, equipos y tareas?
- Considerando que se enfocan en proyectos de gran magnitud, ¿considera que es fácil la asignación de tareas y coordinar los equipos dentro de la aplicación web?
- ¿Qué le parece la visualización del inventario de maquinaria y materiales?
- Las funciones de añadir, editar o eliminar elementos de la administración de recursos, ¿mejora el control de materiales y maquinarias de los proyectos?
- En la sección de documentos, ¿considera que le provee una manera más conveniente de almacenar los archivos necesarios del proyecto?
- ¿Hay alguna funcionalidad adicional que le gustaría ver en la aplicación para facilitar su trabajo en su empresa?
- ¿Considera que esta aplicación mejorará la gestión de proyectos de construcción? 
- ¿Estaría dispuesto a utilizar esta aplicación en sus proyectos actuales o futuros? ¿Por qué?
- ¿Qué valor agregado cree que esta aplicación podría ofrecer a su negocio?


#### 5.3.2. Registro de Entrevistas

### Segmento objetivo: Grandes empresas 

Link de las entrevistas: https://upcedupe-my.sharepoint.com/:v:/g/personal/u202110385_upc_edu_pe/ERDqhrEbplpDrPbJei0KHiYBFQMHL9QJsRQl3K2-acuVlQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=wkqIyW

Entrevista 1:

![Interview3](/Assets/CHAPTER_V/Fabio%20entrevista%20captura.png)

Nombre de entrevistado: Fabio Velarde<br>
Edad: 26 años<br>
Distrito de residencia: Pueblo Libre<br>
Inicio de la entrevista: 00:00
Duración: 11 minutos

En lo que respecta a la landing page, Fabio Velarde comenta que el diseño le resulta llamativo y elegante. Destaca especialmente la paleta de colores utilizada en la aplicación, la cual considera moderna y atractiva, captando la atención del usuario de manera efectiva. Además, menciona que la distribución de la información está muy bien lograda, permitiendo que sea fácil de entender y ofreciendo una apariencia profesional. En cuanto a la aplicación web en sí, Fabio expresa que le resultó extremadamente sencilla y fácil de utilizar. La interfaz intuitiva facilita la navegación entre las diferentes vistas, permitiendo acceder rápidamente a la información necesaria. La forma en que está organizada la información y las opciones disponibles para cada tabla son, según él, aspectos que ayudan significativamente a mejorar la eficiencia en la gestión de la información de los proyectos de construcción. Al final de la entrevista, Fabio nos comparte una sugerencia importante para futuras mejoras. Señala que, en la sección de Gestión de Recursos, sería beneficioso incluir una funcionalidad adicional: la visualización del costo total de los alquileres de las máquinas. Considera que esta característica permitiría a los usuarios presupuestar de manera más precisa a largo plazo, proporcionando una visión más completa de los gastos asociados con el equipo alquilado.<br>

Entrevista 2:

![Validation Interview 2](/Assets/ValidationInterview1.png)

Nombre de entrevistada: Andrea Loli <br>
Edad: 25 años <br>
Inicio de entrevista: 11:30 <br>
Duración: 8 minutos <br>

La arquitecta Andrea Loli nos comentó que la landing page es de su agrado porque es bastante intuitiva. Los botones están posicionados en un lugar que suele ser esperado, por ejemplo, que el toolbar esté en la parte de arriba y que, al hacer click, lleve a la sección deseada. Explica que suele tener problemas con otro tipo de páginas porque tienen mucha información y es difícil saber qué es lo que brinda el producto. Sin embargo, menciona que nuestra página contiene lo necesario y entiende a la perfección cómo funciona BuildSphere. Asimismo, considera que la página es bastante profesional y llama la atención debido a la paleta de colores utilizada. Después, continuamos con la aplicación web. Al igual que con la landing page, ella nos menciona que la aplicación era profesional e intuitiva. Considera que es muy útil para su empresa debido al orden y manejo recursos que brindaria. También, el manejo de documentos es extremadamente útil para ella porque cuenta con muchos archivos para cada proyecto dentro de su computadora y llega a ser confuso. Es por eso que considera que la aplicación permitiría que avancen más rápido ya que toda la información de cada proyecto estaría en orden.

#### 5.3.3. Evaluaciones según heurísticas

#### UX Heuristics & Principles Evaluation

##### Usability – Inclusive Design – Information Architecture

##### CARRERA : Ingeniería de Software

##### CURSO : Desarrollo de Aplicaciones Open Source

##### SECCIÓN : Código de la sección

##### PROFESORES : Todos

##### AUDITOR : AUDIT

##### CLIENTE(S) : ConstruTech


SITE o APP A EVALUAR:

###### BuildSphere

TAREAS A EVALUAR:

El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:

1. Registro de un usuario nuevo

2. Publicación de un proyecto

3. Creación de un nuevo proyecto

4. Inspección del inventario de un proyecto

5. Creación de maquinarias y materiales

6. Inspección de trabajadores, equipos y tareas

7. Creación de trabajador

8. Creación de equipo

9. Asignación de tarea

10. Inspección de documentos

11. Creación de documentos

12. Inspección de soporte

No están incluidas en esta versión de la evaluación las siguientes tareas:

1. Compartir proyectos entre usuarios

2. Pre-visualización de documentos

3. Administración de horarios de trabajadores

4. Guardar equipos para integrar en otros proyectos

5. Guardar trabajadores para integrar en otros proyectos

6. Compartir material o maquinaria entre proyectos



ESCALA DE SEVERIDAD:

Los errores serán puntuados tomando en cuenta la siguiente escala de severidad

| Nivel | Descripción                                                                                                                                                                                                  |
| ----- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1     | Problema superficial: puede ser fácilmente superador por el usuario ó ocurre con muy poco<br><br>frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo.                         |
| 2     | Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de<br><br>superar para el usuario. Se le debería asignar una prioridad baja resolverlo de cara al siguiente<br><br>release |
| 3     | Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es<br><br>importante que sean corregidos y se les debe asignar una prioridad alta.                                       |
| 4     | Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de<br><br>la herramienta. Es imperativo que sea corregido antes del lanzamiento.                                     |



TABLA RESUMEN:

|   |   |   |   |
|---|---|---|---|
|#|Problema|Escala de severidad|Heurística/Principio violada(o)|
|1|No hay un diseño ordenado en la pestaña de “iniciar sesión”|2|Estética y diseño minimalista|
|2|No hay un control para regresar a la pestaña de proyectos|4|Libertad y control por parte del usuario|
|3|No hay un feedback visual para el usuario en cuanto a los ítems dentro del sistema (subida de archivos, estado de maquinarias, estado de tarea, etc)|2|Visibilidad del estado del sistema|




##### DESCRIPCIÓN DE PROBLEMAS:

###### PROBLEMA #1: No hay un diseño ordenado en la pestaña de “iniciar sesión”

Severidad: 2

Heurística violada: Usabilidad - Estética y diseño minimalista

Problema:

Al momento de ingresar a la primera pestaña de la página web, se muestra una pestaña de registro e inicio de sesión poco estilizada y no acorde al diseño de todo el sistema.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXezxFhS0K6vpSQ6IGQkqQ5BUKu4m5aoF65NkRRlH0BsFDtH7bjmYNfCQv1Fnolh3jDUwwjszN24_ZC-aCdFV6ZdpdEefg7kqCU5x0Henak_YMauaUbh7S4FSRxwaR6DlgxQvamdck7W6aUO9_b5tiLveG1z?key=VZ3a3Qx_OHYUABNh-GBNKg)

Recomendación:

Realizar una pestaña visualmente atractiva para el usuario.



###### PROBLEMA #2: No hay un control para regresar a la pestaña de proyectos

Severidad: 4

Heurística violada: Usabilidad - Libertad y control por parte del usuario

Problema:

Al momento de estar navegando por un proyecto y sus pestañas de control del mismo, no se puede regresar a la pestaña de la lista de proyectos. No hay un botón que permita al usuario volver a la pestaña anterior para ingresar a otro proyecto.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXciZA_C99QtVh7XtDntiMSDaVh9Ca8LXKFWYP_ROftCd5SPchM3Krqlbwp4hgZEWLy1d2DUl50GqvUCdh7GZG4O3vtDWy9OxPsdlf-9WrF7TwF5OA5YpOkzHhM10nwJkAOgPFDnkqthUGqE8B2r9V7cRi8?key=VZ3a3Qx_OHYUABNh-GBNKg)

Recomendación:

Lo más práctico es que se pueda añadir un botón en la barra lateral para que el usuario pueda regresar a la pestaña anterior. De tal manera que pueda tener más libertad a la hora de navegar por la página web.



###### PROBLEMA #3: No hay un feedback visual para el usuario en cuanto a los ítems dentro del sistema (subida de archivos, estado de maquinarias, estado de tarea, etc).

Severidad: 2

Heurística violada: Usabilidad - Estética y diseño minimalista

Problema:

Al momento de crear un ítem en cualquiera de las pestañas de maquinarias, trabajadores, materiales o documentación, no hay un feedback para que el usuario sepa si todo el proceso se ha realizado correctamente. Lo que deja una incertidumbre.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfR-3PVCRsD6FnpDzfMxHLBrLhFJBFaL9uvfYAOPHF81WktMnKWuTYPRJ5EeREJnU50gW0m0dpO_veSBQyjwMRr_IEd0-6TUyvw2m4MEqOTSqCj-irET8nEu7VRpzdHXWhT7t5boNp2uGTvzm5tAykFtY8Q?key=VZ3a3Qx_OHYUABNh-GBNKg)

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdPZmih2io_TBZC3YlFxOlkz9HxEzFxGA1nwwZz0lYHsoD31a_v6AjtiMx_M5aZsELLGGCzvxF4AaBBl25JurBDfmP1I4xCvNkmuMGEOiIC0Pksmn2LV0XhtY3X-_4j8eVqFyqrwHqQUG5dLU00l6WuKxc?key=VZ3a3Qx_OHYUABNh-GBNKg)

Recomendación:

Realizar una notificación que le diga al usuario “El documento se ha subido correctamente” o, en caso contrario, “Fallo al subir documento”. Así como este ejemplo para las diferentes pestañas del sistema.

## 5.4. Video About-the-Product

En esta sección se incluye el video about the producto que presenta las funcionalidades principales de la aplicación BuildSphere a los usuarios potenciales.
A continuación, se incluye el link del video about the producto:
- Microsoft Stream: https://upcedupe-my.sharepoint.com/:v:/g/personal/u201923446_upc_edu_pe/ESZlggMojwJHgLuM5ZMZXIQBA-tobRBdjl0ZcXenriYJ6A?e=TEgAEd&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- Youtube: https://youtu.be/w_YDBBP68yI?si=eOelgDSnjojODMkg

![](/Assets/CHAPTER_V/Captura%20about%20the%20product.png)

## 5.5. Video About-the-Team

En esta sección se incluye el video about the team que presenta los miembros  del desarrollo la aplicación BuildSphere.
A continuación, se incluye el link del video about the team:
- Microsoft Stream: https://upcedupe-my.sharepoint.com/:v:/g/personal/u201923446_upc_edu_pe/ES2NsddXAKdMrHbn_zGdtNEB4NF16QtMnQgMALt2l_sEKQ?e=2JEp7o&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D
- Youtube: https://www.youtube.com/watch?v=6fO5tnMJuW0

![](/Assets/CHAPTER_V/About%20the%20team.png)

### Bibliografía 


### Conclusiones 
- La startup ConstruTech tiene el potencial de revolucionar el mercado al ofrecer una solución más accesible y aprovechar el sector de la construcción. una plataforma intuitiva y eficiente con una profunda comprensión de las necesidades del usuario
-  Es muy importante que la página principal de BrainWabe sea intuitiva. Mejorando la facilidad de uso con botones fáciles de entender, una navegación suave y un diseño atractivo, BrainWabe anima a más personas a usar su servicio. Al ofrecer este servicio, el proyecto se convertirá en una opción para quienes buscan gestionar su proyecto.
- La documentación de los servicios y endpoints desarrollados se ha presentado de manera clara y detallada, lo cual es fundamental para facilitar la comprensión y el uso por parte de los usuarios y desarrolladores.
- La evaluación de las heurísticas de UX identificó varios puntos críticos que afectan la experiencia del usuario, como la falta de feedback visual y la navegación poco clara. Estos problemas se han abordado en el desarrollo del spring 3 y 4.
