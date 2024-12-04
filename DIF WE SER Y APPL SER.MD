https://parceljs.org/
Aquí tienes una tabla que resume las diferencias entre un **Web Server** (Servidor Web) y un **Application Server** (Servidor de Aplicaciones):

| **Característica**                | **Web Server**                                      | **Application Server**                                |
|------------------------------------|-----------------------------------------------------|-------------------------------------------------------|
| **Función principal**              | Servir contenido estático (HTML, CSS, imágenes, etc.) y manejar peticiones HTTP. | Ejecutar aplicaciones dinámicas, gestionar la lógica de negocio y las peticiones de clientes. |
| **Tipos de contenido**             | Principalmente contenido estático (HTML, imágenes, archivos CSS, JavaScript). | Contenido dinámico generado por aplicaciones (Java, .NET, PHP, etc.). |
| **Protocolo principal**            | HTTP/HTTPS                                           | HTTP/HTTPS, y otros protocolos como JMS, RMI, EJB. |
| **Ejemplos comunes**               | Apache HTTP Server, Nginx, Microsoft IIS            | Apache Tomcat, JBoss, GlassFish, WebLogic, WildFly. |
| **Capacidades de procesamiento**  | Procesa solicitudes simples (requiere poca o ninguna lógica de negocio). | Procesa solicitudes más complejas, como consultas a bases de datos y ejecución de lógica de negocio. |
| **Soporte para tecnologías**       | Principalmente HTML, CSS, JavaScript, y otros archivos estáticos. | Soporta lenguajes de programación y marcos como Java (JSP, Servlets), .NET, PHP, etc. |
| **Interacción con bases de datos** | Generalmente no interactúa directamente con bases de datos. | Puede gestionar la interacción con bases de datos y otros recursos de backend. |
| **Capa en el modelo OSI**          | Capa de presentación (capa 7, HTTP)                  | Capa de aplicación (capa 7, lógica de negocio). |
| **Escalabilidad**                  | Generalmente utilizado para manejar un alto volumen de solicitudes estáticas de manera eficiente. | Escala para manejar aplicaciones dinámicas y la lógica de negocio a través de múltiples instancias o clústeres. |
| **Dependencia de otros servicios** | Suele depender de un servidor de aplicaciones para ejecutar lógica dinámica. | Puede incluir un servidor web integrado o depender de uno externo. |

### Resumen:
- **Web Server**: Se especializa en manejar y servir contenido estático, como archivos HTML, imágenes y CSS. Es eficiente para manejar grandes cantidades de solicitudes HTTP simples.
- **Application Server**: Se centra en ejecutar aplicaciones y lógica de negocio dinámica, interactuando con bases de datos, generando contenido dinámico y soportando lenguajes de programación para aplicaciones más complejas.

Un **servidor de aplicaciones** a menudo incluye las funcionalidades de un **servidor web**, pero va más allá al proporcionar un entorno completo para ejecutar y gestionar aplicaciones dinámicas.
