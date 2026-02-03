# Literalura - Challenge Oracle Next Education

**Literalura** es una aplicación de consola desarrollada en Java utilizando **Spring Boot**. Su función principal es permitir la búsqueda de libros mediante la API externa de **Gutendex**, permitiendo al usuario registrar libros y autores en una base de datos local para su posterior consulta y filtrado.

## 🚀 Funcionalidades

La aplicación ofrece un menú interactivo con las siguientes opciones:
1. **Buscar libro por título**: Consulta la API de Gutendex y registra el libro (y su autor) si no existen en la base de datos.
2. **Listar libros registrados**: Muestra todos los libros almacenados localmente.
3. **Listar autores registrados**: Muestra la lista de autores guardados.
4. **Listar autores vivos**: Filtra autores que estaban vivos en un año específico.
5. **Listar libros por idioma**: Permite buscar libros filtrando por siglas de idioma (es, en, fr, pt).

## 🛠️ Tecnologías utilizadas

* **Java 17** o superior.
* **Spring Boot**: Framework principal para la configuración y ejecución.
* **Spring Data JPA**: Para la persistencia y mapeo de datos.
* **Jackson**: Para el parseo de datos JSON provenientes de la API.
* **HttpClient**: Para realizar las peticiones a la API externa.

## 📋 Requisitos previos

Para ejecutar este proyecto, necesitarás:
* Tener instalado un **IDE** (como IntelliJ IDEA, basándose en el archivo `.iml` detectado).
* Configurar una base de datos relacional compatible con JPA (como PostgreSQL).
* Configurar el archivo `src/main/resources/application.properties` con tus credenciales de base de datos.

## ⚙️ Configuración

Asegúrate de incluir las siguientes propiedades en tu archivo de configuración para la conexión a la base de datos:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/tu_base_de_datos
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña
spring.jpa.hibernate.ddl-auto=update
