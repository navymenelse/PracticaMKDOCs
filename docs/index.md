# MkDocs: documentación clara y fácil de mantener

MkDocs es un **generador de sitios estáticos** orientado a crear documentación. El contenido se escribe principalmente en Markdown, se organiza en archivos y carpetas, y se configura mediante `mkdocs.yml`. Al construir el proyecto, MkDocs convierte esos contenidos en páginas HTML que pueden publicarse en un servidor web o en servicios de alojamiento estático.

Esta página reúne una introducción a MkDocs mediante pestañas, bloques desplegables y enlaces a los módulos del proyecto. Selecciona las pestañas para explorar cada tema.

!!! info "¿Qué significa que sea un sitio estático?"
    Las páginas se preparan al generar el sitio; no necesitan ejecutar una aplicación ni consultar una base de datos cada vez que una persona las visita. Esto hace que publicar documentación sea sencillo y que el resultado pueda servirse desde muchos servicios web.

## Explora MkDocs

=== "Descripción"

    ### ¿Qué es MkDocs?

    MkDocs es una herramienta libre y de código abierto para transformar documentos Markdown en un sitio de documentación. Su configuración central suele estar en `mkdocs.yml`, donde se indican, entre otras cosas, el nombre del sitio, el tema, la navegación y las extensiones de Markdown.

    Un proyecto típico tiene esta estructura:

    ```text
    proyecto/
    ├── mkdocs.yml
    └── docs/
        ├── index.md
        └── guia.md
    ```

    La carpeta `docs/` contiene las páginas, imágenes y otros recursos del sitio. El tema determina la presentación; por ejemplo, **Material for MkDocs** aporta navegación, búsqueda, paletas de color y componentes visuales.

=== "Historia"

    ### Origen y evolución

    MkDocs apareció en 2014 como una alternativa sencilla para crear documentación de proyectos. Su propuesta combinó tres elementos: escribir en Markdown, describir la configuración en YAML y generar un sitio web estático. El proyecto es de código abierto y su desarrollo continúa en comunidad.

    Con el tiempo, su ecosistema incorporó temas y extensiones que permiten adaptar el diseño y ampliar Markdown sin tener que construir desde cero un sistema de documentación. **Material for MkDocs** es uno de esos temas: es un proyecto independiente que se integra con MkDocs y aporta una interfaz moderna y componentes interactivos.

    === "Una evolución en tres ideas"

        1. **Contenido sencillo:** escribir y organizar documentación en Markdown.
        2. **Generación automática:** convertir los documentos en páginas web.
        3. **Personalización:** añadir temas, extensiones y estilos según las necesidades del proyecto.

=== "Utilidad"

    ### ¿Para qué sirve?

    MkDocs sirve para crear y mantener documentación navegable sin redactar cada página directamente en HTML. Permite dividir la información en archivos pequeños, agruparlos en una estructura lógica y generar el sitio completo con un comando.

    ```bash
    mkdocs serve
    ```

    Este comando inicia un servidor local de vista previa, útil para revisar los cambios mientras se trabaja. Para generar la versión lista para publicar:

    ```bash
    mkdocs build
    ```

    La navegación del sitio se define en `mkdocs.yml`, y los enlaces entre documentos ayudan a conectar conceptos relacionados.

=== "Aplicaciones"

    ### ¿En qué proyectos se puede utilizar?

    MkDocs es apropiado cuando se necesita publicar información organizada en páginas:

    - **Manuales de usuario:** instrucciones, preguntas frecuentes y guías de inicio.
    - **Documentación técnica:** instalación, configuración, arquitectura y resolución de problemas.
    - **Documentación de código y API:** explicación de módulos, ejemplos y referencias.
    - **Material educativo:** apuntes, módulos, actividades y recursos de un curso.
    - **Proyectos y equipos:** procedimientos internos, decisiones y guías de contribución.
    - **Portafolios:** presentación de trabajos, conocimientos y herramientas utilizadas.

    La documentación puede mantenerse junto al código del proyecto y revisarse con el mismo flujo de control de versiones.

=== "Ventajas"

    ### ¿Qué ventajas ofrece?

    | Ventaja | Qué aporta |
    | --- | --- |
    | Escritura legible | Markdown permite centrarse en el contenido sin escribir HTML para cada página. |
    | Organización | Los archivos y la navegación se pueden estructurar por temas y secciones. |
    | Vista previa local | `mkdocs serve` facilita comprobar los cambios antes de publicar. |
    | Publicación flexible | El resultado es un sitio estático que puede alojarse en distintos servicios compatibles. |
    | Personalización | Los temas y las extensiones adaptan el aspecto y amplían el formato. |
    | Mantenimiento | Los cambios en texto y configuración pueden controlarse con Git. |
    | Accesibilidad al equipo | Los archivos de texto son fáciles de revisar, compartir y modificar. |

    !!! tip "Una ventaja práctica"
        Al separar el contenido de la presentación, puedes reorganizar páginas o cambiar el tema sin tener que rehacer toda la documentación.

## Flujo de trabajo habitual

1. **Crear** las páginas Markdown dentro de `docs/`.
2. **Organizar** el sitio y sus opciones en `mkdocs.yml`.
3. **Previsualizar** con `mkdocs serve` y corregir enlaces o contenido.
4. **Generar** el sitio con `mkdocs build`.
5. **Publicar** los archivos generados en un servicio de alojamiento web estático.

??? question "¿MkDocs necesita una base de datos para mostrar la documentación?"
    No. MkDocs genera páginas estáticas durante la compilación. Para mostrar el sitio publicado, el servidor entrega esos archivos al navegador. Algunas funciones externas podrían requerir servicios adicionales, pero no son necesarias para el funcionamiento básico.

??? question "¿Qué papel tiene Material for MkDocs?"
    MkDocs genera y organiza el sitio; Material for MkDocs es un tema que define su apariencia e incorpora elementos de interfaz, como navegación, búsqueda, pestañas y bloques desplegables.

## Módulos de este proyecto

En este proyecto se exploran herramientas y conceptos relacionados con el desarrollo y la organización del trabajo:

- [Módulo de MkDocs](ModuloMkDocs.md): configuración y generación de documentación.
- [Módulo de Markdown](ModuloMarkdown.md): formato empleado para escribir las páginas.
- [Módulo de Teams](ModuloTeams.md): colaboración y comunicación.
- [Módulo de Trello](ModuloTrello.md): organización visual de tareas.
- [Diagrama de Gantt](ModuloDiagramaGantt.md): planificación temporal.
- [SCRUM](ModuloSCRUM.md): marco de trabajo ágil.
- [Práctica final](ModuloPracticaFinal.md): aplicación de lo aprendido en el proyecto.

## En resumen

MkDocs ofrece una forma directa de convertir archivos Markdown en documentación web. Su configuración sencilla, la posibilidad de usar distintos temas y extensiones, y su salida estática lo hacen útil para proyectos educativos, técnicos y profesionales. Con Material for MkDocs, además, es posible presentar la información con una navegación clara y componentes interactivos como los que aparecen en esta página.