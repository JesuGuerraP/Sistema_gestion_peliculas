# Sistema de Gestión de Películas

Aplicación de consola para gestionar información sobre películas. Este sistema permite realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre una base de datos de películas y está diseñado con un enfoque orientado a objetos.

## Características
- **Gestión de Películas**:
  - Crear nuevas películas.
  - Listar todas las películas disponibles.
  - Actualizar información de películas existentes.
  - Eliminar películas del sistema.
- **Interfaz de Consola**:
  - Menú interactivo para realizar operaciones fácilmente.
- **Persistencia**:
  - Datos almacenados de forma segura en una base de datos, garantizando su disponibilidad entre sesiones.
- **Diseño Modular**:
  - Estructura basada en clases y métodos para facilitar la escalabilidad y el mantenimiento.

## Tecnologías Utilizadas
- **Lenguaje**: Java
- **Base de Datos**: MySQL
- **Conexión**: JDBC

## Instalación
1. Clona este repositorio:
   ```bash
   git clone https://github.com/JesuGuerraP/Sistema_gestion_peliculas.git
Configura la base de datos MySQL:

Crea una base de datos y tabla con el siguiente script SQL:
sql
Copiar código
CREATE DATABASE MovieManagementDB;
USE MovieManagementDB;

CREATE TABLE movies (
    id INT AUTO_INCREMENT PRIMARY KEY,
    title VARCHAR(255) NOT NULL,
    genre VARCHAR(100) NOT NULL,
    director VARCHAR(100),
    release_date DATE,
    rating DECIMAL(3, 1)
);
Asegúrate de configurar correctamente el usuario y la contraseña de MySQL en la clase de conexión.
Abre el proyecto en tu IDE de Java preferido.

Compila y ejecuta el archivo principal (Main.java).

Uso
Ejecuta la aplicación desde la consola.
Utiliza las opciones del menú para realizar las operaciones deseadas.
Ejemplo de Menú
text
Copiar código
1. Agregar Película
2. Listar Películas
3. Actualizar Película
4. Eliminar Película
5. Salir
