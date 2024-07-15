# nodejs-first-project

##  1. ¿Qué es el filesystem (fs) en Node.js y para qué se utiliza?

El módulo ‘fs’ en Node.js proporciona una API para interactuar con el sistema de archivos. Permite realizar operaciones como leer, escribir, modificar y eliminar archivos y directorios. Es esencial para aplicaciones que necesitan manipular archivos directamente en el sistema.

## 2. ¿Qué es un middleware en Express y cuál es su propósito?

Un middleware en Express es una función que se ejecuta durante el ciclo de vida de una solicitud HTTP. Su propósito es interceptar y modificar las solicitudes y respuestas antes de que lleguen a los controladores de ruta o después de que salgan de ellos. Los middlewares pueden ser utilizados para tareas como manejo de errores, autenticación, validación de datos, logging, etc.

## 3. ¿Qué es un endpoint en una API RESTful y cuál es su función?

Un endpoint en una API RESTful es una URL específica donde un cliente puede acceder a los recursos de la API. Cada endpoint está asociado a una función específica, como obtener datos, crear nuevos datos, actualizar datos existentes o eliminar datos. Los endpoints permiten a los clientes interactuar con el servidor de manera organizada y predecible.

## 4. ¿Qué son los verbos HTTP y cuáles son los más comunes?

Los verbos HTTP, también conocidos como métodos HTTP, definen las acciones que se pueden realizar sobre los recursos en una API RESTful. Los verbos HTTP más comunes son:

•	GET: Recuperar datos de un recurso.
•	POST: Enviar datos para crear un nuevo recurso.
•	PUT: Actualizar un recurso existente.
•	DELETE: Eliminar un recurso existente.
•	PATCH: Aplicar modificaciones parciales a un recurso.

## 5. ¿Qué es JSON y por qué es utilizado en las API RESTful?

JSON (JavaScript Object Notation) es un formato de datos ligero y fácil de leer para los humanos y de generar y parsear para las máquinas. Es ampliamente utilizado en las API RESTful porque es independiente del lenguaje de programación, compacto y fácil de entender. Permite una transferencia eficiente de datos entre el cliente y el servidor.

## 6. En lo que Respecta al Envío de Datos a lo Largo de los Verbos HTTP

### ¿Qué es el body de una petición?

El body de una petición es la parte de la solicitud HTTP donde se envían los datos al servidor. Es utilizado principalmente con los verbos ‘POST’ y ‘PUT’ para enviar datos que se desean almacenar o actualizar en el servidor.

### ¿Qué es el body de una respuesta?

El body de una respuesta es la parte de la respuesta HTTP que contiene los datos devueltos por el servidor al cliente. Puede incluir información en varios formatos, como JSON, HTML, XML, etc.

### ¿Qué es el query de una petición?

El query de una petición es la parte de la URL que contiene parámetros de consulta, proporcionando datos adicionales a la solicitud en forma de pares clave-valor. Se utiliza para filtrar, ordenar y paginar resultados sin afectar la estructura de la URL base.

### ¿Qué es el params de una petición?

El params de una petición se refiere a los parámetros de ruta que se definen en la URL de la solicitud. Estos parámetros permiten identificar recursos específicos dentro de una ruta. Por ejemplo, en la URL ‘/tasks/:id’, ‘:id’ es un parámetro de ruta.


## 7. En lo que Respecta al Verbo POST

### ¿Qué es un verbo POST y cuál es su propósito?
El verbo ‘POST’ se utiliza para enviar datos al servidor para crear un nuevo recurso. Su propósito principal es agregar nuevos datos al servidor.
¿Cuándo se utiliza un verbo POST?
Se utiliza un verbo POST cuando se necesita crear un nuevo recurso en el servidor, como al registrar un nuevo usuario, agregar un nuevo artículo a un blog, etc.

### ¿En qué se diferencia un verbo POST de los otros verbos HTTP como GET, PUT y DELETE?

•	POST se utiliza para crear nuevos recursos.
•	GET se utiliza para recuperar recursos existentes.
•	PUT se utiliza para actualizar recursos existentes.
•	DELETE se utiliza para eliminar recursos existentes.

### ¿Cómo se envían datos en un verbo POST?

Los datos se envían en el cuerpo de la solicitud (body) en un formato como JSON, XML, o ‘form-data’, dependiendo de la configuración de la API y el cliente.

## 8. En lo que Respecta al Verbo GET

### ¿Qué es un verbo GET y cuál es su propósito?

El verbo ‘GET’ se utiliza para recuperar datos de un recurso en el servidor. Su propósito es obtener información sin realizar cambios en el servidor.

### ¿Cuándo se utiliza un verbo GET?

Se utiliza un verbo ‘GET’ cuando se necesita obtener información o datos de un servidor, como al visualizar una lista de tareas, detalles de un producto, etc.

### ¿En qué se diferencia un verbo GET de los otros verbos HTTP como POST, PUT y DELETE?

•	GET se utiliza para recuperar datos sin modificar el estado del servidor.
•	POST se utiliza para crear nuevos recursos.
•	PUT se utiliza para actualizar recursos existentes.
•	DELETE se utiliza para eliminar recursos.

## 9. En lo que Respecta al Verbo PUT

### ¿Qué es un verbo PUT y cuál es su propósito?

El verbo ‘PUT’ se utiliza para actualizar un recurso existente en el servidor. Su propósito es enviar datos para reemplazar el estado actual del recurso.

### ¿Cuándo se utiliza un verbo PUT?

Se utiliza un verbo ‘PUT’ cuando se necesita actualizar completamente un recurso existente en el servidor.

### ¿En qué se diferencia un verbo PUT de los otros verbos HTTP como POST, GET y DELETE?

•	PUT se utiliza para actualizar completamente un recurso existente.
•	POST se utiliza para crear nuevos recursos.
•	GET se utiliza para recuperar recursos.
•	DELETE se utiliza para eliminar recursos.

## 10. En lo que Respecta al Verbo DELETE

### ¿Qué es un verbo DELETE y cuál es su propósito?

El verbo ‘DELETE’ se utiliza para eliminar un recurso existente en el servidor. Su propósito es eliminar datos.

### ¿Cuándo se utiliza un verbo DELETE?
Se utiliza un verbo ‘DELETE’ cuando se necesita eliminar un recurso existente en el servidor.

### ¿En qué se diferencia un verbo DELETE de los otros verbos HTTP como POST, GET y PUT?

•	DELETE se utiliza para eliminar recursos.
•	POST se utiliza para crear nuevos recursos.
•	GET se utiliza para recuperar recursos.
•	PUT se utiliza para actualizar completamente recursos.

## 11. ¿Qué es un status code y cuáles son los más comunes?

Un status code es un código numérico que el servidor envía en respuesta a una solicitud HTTP para indicar el resultado de la operación solicitada. Los códigos de estado más comunes son:

•	200 OK: La solicitud fue exitosa.
•	201 Created: La solicitud fue exitosa y se creó un nuevo recurso.
•	204 No Content: La solicitud fue exitosa pero no hay contenido que devolver.
•	400 Bad Request: La solicitud es inválida o malformada.
•	401 Unauthorized: La solicitud requiere autenticación.
•	403 Forbidden: El servidor entendió la solicitud, pero se niega a autorizarla.
•	404 Not Found: El recurso solicitado no fue encontrado.
•	500 Internal Server Error: El servidor encontró un error al procesar la solicitud.

## 12. ¿Cuáles son los status code más comunes para el verbo POST?

•	201 Created: Indica que el recurso fue creado exitosamente.
•	400 Bad Request: Indica que hubo un error en la solicitud.

### 13. ¿Cuáles son los status code más comunes para el verbo GET?

•	200 OK: Indica que la solicitud fue exitosa y el recurso fue devuelto.
•	404 Not Found: Indica que el recurso solicitado no fue encontrado.

## 14. ¿Cuáles son los status code más comunes para el verbo PUT?

•	200 OK: Indica que la actualización fue exitosa.
•	204 No Content: Indica que la actualización fue exitosa y no hay contenido que devolver.
•	400 Bad Request: Indica que hubo un error en la solicitud.
•	404 Not Found: Indica que el recurso a actualizar no fue encontrado.

## 15. ¿Cuáles son los status code más comunes para el verbo DELETE?

•	200 OK: Indica que la eliminación fue exitosa.
•	204 No Content: Indica que la eliminación fue exitosa y no hay contenido que devolver.
•	404 Not Found: Indica que el recurso a eliminar no fue encontrado.

