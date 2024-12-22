Hola y bienvenido!

Objetivo: Crear una API para la gestión de un hotel que permita manejar reservas, habitaciones, pagos, clientes y administradores. 
Deberás implementar la lógica de negocio, estructuras de datos y endpoints para manejar las distintas funcionalidades del sistema. 
Este ejercicio ayudará a mejorar las habilidades en la creación de APIs RESTful, manejo de bases de datos y comprensión de las mejores prácticas en arquitectura de software.

Requerimientos Funcionales:
Clientes:

Crear, leer, actualizar y eliminar clientes.
Un cliente debe tener al menos los siguientes campos:
  ID (único)
  Nombre
  Apellidos
  Correo electrónico
  Número de teléfono
  Habitaciones:

Crear, leer, actualizar y eliminar habitaciones.


Una habitación debe tener al menos los siguientes campos:
  ID (único)
  Número de habitación
  Tipo de habitación (simple, doble, suite)
  Precio por noche
  Estado (disponible, ocupada, en mantenimiento)
  
Reservas:
Crear, leer, actualizar y cancelar reservas.
Una reserva debe tener al menos los siguientes campos:
  ID (único)
  ID del cliente
  ID de la habitación
  Fecha de inicio de la reserva
  Fecha de fin de la reserva
  Estado de la reserva (pendiente, confirmada, cancelada)

Pagos:
Registrar pagos asociados a una reserva.
Un pago debe tener al menos los siguientes campos:
  ID (único)
  ID de la reserva
  Monto
  Fecha de pago
  Método de pago (tarjeta, efectivo, transferencia)
  
Administradores:
Crear, leer, actualizar y eliminar administradores.
Un administrador debe tener al menos los siguientes campos:
  ID (único)
  Nombre
  Correo electrónico
  Contraseña (hasheada)
  Rol (admin, superadmin)
  
Autenticación y Autorización:
  Implementar autenticación para los administradores.
  Sólo los administradores deben poder crear, actualizar o eliminar habitaciones y reservas.
  Los clientes pueden crear y ver sus propias reservas, pero no modificarlas una vez confirmadas.
  
Requerimientos Técnicos:
  Lenguaje: Recomiendo usar Java (Spring Boot) o .NET (ASP.NET Core), aunque puede implementarse en cualquier otro lenguaje que soporte la creación de APIs RESTful. (puedes usar python, C... el que quieras).
  
Base de Datos: Utilizar una base de datos relacional como MySQL, PostgreSQL, o SQL Server.

Estructura de Datos:
Usar objetos de transferencia de datos (DTOs) para manejar la comunicación entre la API y el cliente.
Implementar un mapeo objeto-relacional (ORM) como JPA/Hibernate en Java o Entity Framework en .NET.

Validación: Implementar validaciones para las entradas de los usuarios. Ejemplo: verificar que una reserva no se haga sobre una habitación ocupada.

Documentación: Crear documentación de la API usando Swagger/OpenAPI para que otros desarrolladores puedan entender y probar fácilmente la API.

Pruebas: Implementar pruebas unitarias y de integración para asegurar la funcionalidad y estabilidad de la API.

Desafíos Adicionales:
  Optimización de Consultas: Optimizar las consultas SQL para mejorar el rendimiento, especialmente al manejar un gran número de reservas o habitaciones.
  Gestión de Estados: Implementar lógica para la transición de estados (por ejemplo, de "pendiente" a "confirmada" en una reserva).
  Manejo de Concurrencia: Considerar el manejo de concurrencia en la reserva de habitaciones para evitar sobre-reservas.
  Escalabilidad: Diseñar la API pensando en la escalabilidad, permitiendo la implementación en un entorno distribuido o en la nube.
  Seguridad: Implementar medidas de seguridad como autenticación JWT, cifrado de contraseñas, y protección contra ataques comunes como SQL Injection y XSS.


Entregables:
Código fuente de la API.
Instrucciones para configurar y ejecutar el proyecto localmente.
Documentación de la API (idealmente en Swagger/OpenAPI).
Scripts para crear y poblar la base de datos.
Pruebas unitarias y de integración.

TODO ESTO EN UNA PR CON VUESTRO USUARIO Y UN TEXTO EXPLICANDOLO.
