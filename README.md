# PlatformEngineerHiringTest

# Desafío de Contratación Platform Engineer

Agradecemos tu interés en unirte a nuestro equipo como Ingeniero de Plataforma. Para avanzar en el proceso de selección, te invitamos a participar en el siguiente desafío técnico, que nos permitirá evaluar tus habilidades y enfoque en la resolución de problemas reales.

## Objetivo del Desafío

Tu objetivo es diseñar y desarrollar una aplicación que incluya tanto backend como frontend. Para el backend, puedes considerar Spring Boot, Express/NestJS, o cualquier otra tecnología que prefieras, incluyendo opciones serverless como AWS Lambda. En cuanto al frontend, te recomendamos Next.js, pero eres libre de elegir el framework o biblioteca que mejor se ajuste a tu enfoque de desarrollo.

## Desafío

Blue Express viene creciendo de manera muy acelerada en los últimos años. La experiencia de envío y la cantidad de referencias que tenemos es clave para entender ese crecimiento, pero seamos sinceros, no se crece solo teniendo un gran producto, sino comunicando y teniendo grandes campañas de marketing. 

En esa línea, se quiere dotar al equipo de Marketing de herramientas para poder hacer comunicaciones por canales de mensajería como SMS o Twitter. En estos canales, es muy importante que las comunicaciones sean cortas, así que es necesario desarrollar un acortador de URL.

## Contexto

### ¿Qué es un acortador de URL?

Un acortador de URL es una herramienta esencial en el marketing digital, especialmente en plataformas donde el espacio es limitado, como Twitter o SMS. Este servicio ofrece dos funcionalidades clave:


Es un servicio que permite dos cosas:

1. Acortar URLs Largas:

- ***Funcionamiento***: Un usuario de Marketing introduce una URL larga, como https://envios.bluexpress.cl/courierExpress/#menu=categories.

- ***Resultado***: El servicio genera una versión más corta, como https://bu.ex/XXYYZZ.

2. Redirigir a la URL Original desde la Acortada:

- ***Funcionamiento***: Cuando un usuario final navega a la URL acortada (https://bu.ex/XXYYZZ), el servicio redirige automáticamente a la URL original.

- ***Resultado***: El usuario accede a https://envios.bluexpress.cl/courierExpress/#menu=categories, aunque haya ingresado la versión acortada.

### Beneficios en Marketing

El uso de un acortador de URL permite reducir significativamente la longitud de los mensajes de marketing, lo que es crucial en plataformas con restricciones de caracteres. Por ejemplo:

> Mensaje Original (162 caracteres):

    "No te pierdas las únicas oportunidades que tenemos para tus envios https://envios.bluexpress.cl/courierExpress/#menu=categories"

> Mensaje con URL Acortada (111 caracteres):

    "No te pierdas las únicas oportunidades que tenemos para tus envios https://bu.ex/XXYYZZ"

Esta reducción no solo mejora la estética y legibilidad de los mensajes, sino que también permite incluir información adicional o llamados a la acción dentro del mismo mensaje, maximizando así el impacto de las campañas de marketing.


## ¿Qué te pedimos?

Desarrolla un servicio que cumpla con las siguientes funcionalidades:

- **Generación de URL Corta**: Al recibir una URL larga, el servicio debe proporcionar una versión acortada.
- **Recuperación de URL Original**: Al recibir una URL corta, el servicio debe ser capaz de devolver la URL larga original.
- **Estadísticas de Uso**: El servicio debe poder ofrecer estadísticas sobre las URLs que utilizan este servicio.
- **Alta Escalabilidad**: Capacidad para manejar un gran volumen de solicitudes, con un objetivo de al menos 5.000 peticiones por segundo.
- **Alto Rendimiento**: El 90% de todas las solicitudes deben ser respondidas en menos de 10 ms. La creación de una URL corta debe ser un proceso rápido, idealmente en el orden de 1 segundo.
- **Gestión de URLs Cortas**: Posibilidad de eliminar URLs cortas que ya no son necesarias.
- **Redirección Efectiva**: Asegurar que el usuario sea redirigido hacia la URL larga original al ingresar una URL corta válida en su navegador.
- *IaC*: Idealmente usar IaC . Por ejemplo, Terraform, CloudFormation, etc.

## ¿Qué se validará cuando presentes?

- **Funcionalidad API**: Realizaremos pruebas al API de creación y borrado para confirmar que las URLs cortas se crean y destruyen efectivamente.
- **Pruebas de Navegación**: Usaremos la URL corta en un navegador para verificar la redirección a la URL larga.
- **Resiliencia del Sistema**: Queremos entender cómo responde el sistema ante fallos en los diferentes componentes de la solución desarrollada o integrada.
- **IDP**: Idealmente, la solución debe incluir acceso seguro a través de un IDP como Google, Facebook, etc.

## ¿Qué no hace falta que hagas?
No es necesario desarrollar un sistema de monitoreo completo, ya que esto es un MVP (Producto Mínimo Viable) enfocado en Cloud & Platform.
