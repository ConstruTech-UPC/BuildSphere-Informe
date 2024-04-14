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
[**Netlify**](https://www.netlify.com/): Para llevar a cabo el deployment del landing page, se procedió a vincular el repositorio de Github con Netlify. De este modo, Netlify gestionará de manera automática el deploy del landing page cada vez que exista un nuevo cambio en el repositorio.
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


