# Capítulo V: Product Implementation, Validation & Deployment.

## 5.1. Software Configuration Management.

### 5.1.1. Software Development Environment Configuration.
En esta sección se describirán los productos para el desarrollo de software que han sido implementados para este proyecto. Así mismo, esta sección da su importancia al contar con información relevante para futuros equipos de desarrollo que deseen continuar con el ciclo de vida del producto de software.
### Project Management
- [**Discord**](https://discord.com/): Plataforma que funciona como aplicación web y mobile. Se empleó esta plataforma como medio para las reuniones virtuales, las diversas ceremonias de SCRUM con el equipo.
- [**Trello**](https://trello.com/es): La herramienta es una aplicación web empleada para realizar la asignación de tareas en el formato (do, doing & done). De tal forma que todo el equipo tenga conocimiento de las tareas que se están realizando con el fin de tener un buen proyecto.
### Requirements Management
- [**Trello**](https://trello.com/es): La herramienta nos permite realizar un backlog de equipo y colaborar en el mismo. Adicionalmente, proporciona una vista cómoda respecto a este dejando en claro los puntos de interés o prioridad del equipo.
### Product UI/UX Design
- [**Figma**](https://www.figma.com/): La aplicación web de Figma fue utilizada para desarrollar los wireframes, mockups y mobile applications prototyping de manera colaborativa.
- [**Uxpressia**](https://uxpressia.com/): Se empleó esta aplicación web para la realización de los User Personas, el Customer Journey Map, Empathy Map e Impact Map.
- [**Miro**](https://miro.com/): La aplicación web de Miro ha sido utilizada en el desarrollo de los escenarios mapping y customer journey map
### Software Development
- **Landing Page**: Para la realización del landing page se utilizarán las tecnologías de: HTML5, CSS3 y JavaScript. Además, para realizar un óptimo desarrollo para la forma responsiva, se utilizará el framework de BootStrap.
- **Frontend Web Application**: Para la realización del está sección de nuestra aplicación web se usarán las mismas tecnologías que en el Landing Page. Adicionalmente, nos estaremos apoyando del framework Vue para su realización como librería complementaria de JavaScript.
- **Herramientas:** Node, npm, Vite
### Web Services
Para los diversos servicios web que se desarrollaran, se empleará el estilo de arquitectura RESTful API. Se usará el lenguaje C#, ya que estaremos usando ASP .NET.
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
- [Informe](https://github.com/upc-pre-SI730-2401-SW51-equipo1/ChromaComics)
- [Landing Page](https://github.com/upc-pre-SI730-2401-SW51-equipo1/ChromaComics)
- [Acceptance test](https://github.com/upc-pre-SI730-2401-SW51-equipo1/ChromaComics)
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
**Convenciones de versiones de lanzamiento:**
Para el formato de versiones se aplicará "Semantic Versioning 2.0.0". Donde las versiones siguen el formato de (X.Y.Z). Donde:

- X: Representa una versión mayor. Aquí se encuentran los cambios que no son compatibles con las versiones anteriores.
- Y: Versión menor. Aquí se encuentran los cambios que sí son compatibles con las versiones anteriores.
- Z: Parches y correcciones de errores menores.

**Guía de estilo y convenciones de código fuente:**
- **HTML y CSS**: Se utilizará [Google HTML/CSS Style Guide](https://google.github.io/styleguide/htmlcssguide.html), ya que contiene los formatos que se deben tener en cuenta al trabajar con dichas tecnología.
- **JavaScript:** Se utilizará la [guia de estilos para js](https://google.github.io/styleguide/jsguide.html).
- **Gherkin:** Se usarán las convenciones mencionadas en [Make your Gherkin Specifications More Readable](https://specflow.org/gherkin/gherkin-conventions-for-readable-specifications/).
- **Sprint Boot:** Para las convenciones de se utilizarán las ya mencionadas por el equipo de [Sprint Boot](https://docs.vmware.com/en/VMware-Tanzu-Application-Platform/1.9/tap/spring-boot-conventions-reference-CONVENTIONS.html).
- Java: Con el fin de cumplir los estándares del leguaje, se usará la [guia proporcionada por Oracle](https://www.oracle.com/technetwork/java/codeconventions-150003.pdf) para cumplir con su su correcta nomenclatura.
- .NET Framework: Para cumplir con la guia de estilos, Microsoft también nos proporciona una guia en su propio [repositorio github](https://github.com/dotnet/aspnetcore/wiki/Engineering-guidelines#coding-guidelines).
### 5.1.4. Software Deployment Configuration.
Para el despliege en la plataforma, lo realizaremos de la siguiente manera:
1.  Accedemos  a [Netlify](https://www.netlify.com/) y nos creamos una cuenta (si ya contamos con una cuenta, ingresamos). Luego, realizamos la busqueda de la sección de ''add new site'' e importaremos un proyecto existente con la opción ''Import an existing project''.
2. Seleccionamos cuál será la plataforma con el repositorio donde tenemos el código de nuestra aplicación. En nuestro caso será GitHub.
3. Seleccionamos la organización en donde se instalará el deploy de nuestra página web
4. Finalmente, indicamos el repositorio y la ruta o branch de la cuál se realizará el despliegue.