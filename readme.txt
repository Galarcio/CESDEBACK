Sistema de Gestión de Citas Médicas

Este es un servicio web desarrollado con Spring Boot y MySQL, que permite la gestión de citas médicas entre pacientes y médicos.

🚀 Tecnologías Utilizadas

Java 17

Spring Boot 3.4.2

Spring Data JPA

MySQL 8

Maven

🛠 Instalación y Configuración

1️⃣ Clonar el Repositorio

  git clone https://github.com/tu_usuario/citas-medicas.git
  cd citas-medicas

2️⃣ Configurar la Base de Datos

Crear la base de datos en MySQL:

CREATE DATABASE citas_medicas;
USE citas_medicas;

Actualizar el archivo src/main/resources/application.properties con tus credenciales:

spring.datasource.url=jdbc:mysql://localhost:3306/citas_medicas?serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=tu_contraseña
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect

3️⃣ Ejecutar el Proyecto

  mvn spring-boot:run

Si la ejecución es exitosa, la aplicación estará corriendo en http://localhost:8080.

📌 Endpoints Disponibles

🔹 Pacientes

GET /pacientes → Obtener todos los pacientes

POST /pacientes → Crear un nuevo paciente

🔹 Médicos

GET /medicos → Obtener todos los médicos

POST /medicos → Crear un nuevo médico