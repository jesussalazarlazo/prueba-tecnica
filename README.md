# Proyecto CreateUser API


## Insignias


## Índice

- [Descripción del Proyecto](#descripción-del-proyecto)
- [Requisitos](#requisitos)
- [Estado del Proyecto](#estado-del-proyecto)
- [Demostración de Funciones y Aplicaciones](#demostración-de-funciones-y-aplicaciones)
- [Acceso al Proyecto](#acceso-al-proyecto)
- [Configuración de la Base de Datos](#configuración-de-la-base-de-datos)
- [Compilar y Ejecutar el Proyecto](#compilar-y-ejecutar-el-proyecto)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Personas Contribuyentes](#personas-contribuyentes)
- [Personas Desarrolladoras del Proyecto](#personas-desarrolladoras-del-proyecto)
- [Licencia](#licencia)

## Descripción del Proyecto

Este proyecto es una API REST para la gestión de usuarios, que permite crear nuevos usuarios, realizar validaciones y manejar errores de manera efectiva. Proporciona un conjunto de endpoints para interactuar con los datos de los usuarios.


## Estado del Proyecto

- **En Desarrollo**: El proyecto está en fase de desarrollo activo y se están implementando nuevas funcionalidades.
- **Version**: 1.0.0

## Requisitos

- **JDK**: Java 11 o superior
- **Maven**: Para la gestión de dependencias
- **h2**: Base de datos (o cualquier otra base de datos que estés usando)
- **Postman**: Herramienta opcional para probar la API

## Estado del Proyecto

- **En Desarrollo**: El proyecto está en fase de desarrollo activo y se están implementando nuevas funcionalidades.
- **Versión**: 1.0.0

## Demostración de Funciones y Aplicaciones

![Demostración](ruta/a/tu/demo.jpg)  <!-- Reemplaza con la URL de tu imagen de demostración -->

### Ejemplo de Uso

- **Crear un usuario**: `POST /api/users`

**Cuerpo de la solicitud**:

```json
{
"name": "Jesus Salazar",
"email": "jesussalaz12a33r@pepe.com.pe",
"password": "Jesus123",
"phones": [
        {
            "number": "935602618",
            "citycode": "123",
            "countrycode": "5152"
        }
    ]
}
```

**Respuesta Exitosa**:


```json
Código de estado: 201 Created
Cuerpo de la respuesta:

{
    "id": 4,
    "name": "Jesus Salazar",
    "email": "jesussalaz@pepe.com.pe",
    "password": "Jesus123",
    "created": "01/10/2024",
    "modified": "01/10/2024",
    "lastLogin": "01/10/2024",
    "token": "290a6a47-d94d-4220-81c0-a4d1a48bcc7b",
    "phones": [
        {
            "id": 2,
            "number": "935602618",
            "citycode": "123",
            "countrycode": "5152"
        }
    ],
    "active": true
}
```
	
 ### Errores Comunes- **
400 Bad Request: Si hay errores de validación.
409 Conflict: Si el correo ya está registrado.
500 Internal Server Error: Para errores no manejados.

### Acceso al Proyecto

git clone <URL_DEL_REPOSITORIO>
cd createuser

## Instalación

1. **Clonar el repositorio**

   bash
   git clone <https://github.com/jesussalazarlazo/prueba-tecnica>
   cd createuser
   
  ## Actualiza las credenciales en
  # Configuración de la base de datos H2
	spring.datasource.url=jdbc:h2:mem:testdb;DB_CLOSE_DELAY=-1;DB_CLOSE_ON_EXIT=FALSE
	spring.datasource.driver-class-name=org.h2.Driver
	spring.datasource.username=sa
	spring.datasource.password=

# Habilitar la consola web de H2
spring.h2.console.enabled=true

# Configuración de JPA
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.jpa.hibernate.ddl-auto=create-drop

#tecnologías-utilizadas
**Java: JDK 11 o superior
**Spring Boot: Para la creación de la API REST
**Maven: Para la gestión de dependencias
**H2Dialect: Base de datos utilizada
**Postman: Herramienta para probar la API

#Personas Contribuyentes
**Jesus Salazar Lazo - Desarrollador Principal

#Personas Desarrolladoras del Proyecto
**Jesus Salazar Lazo: Desarrollador Principal


#Licencia
**Este proyecto está bajo la Licencia MIT. Para más detalles, consulta el archivo LICENSE.

### Instrucciones:
`README.md`
