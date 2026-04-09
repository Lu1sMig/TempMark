# 🚀 S03-26-Equipo-06-Web-App-Development
CMS para gestionar y publicar testimonios con soporte multimedia.

## 📌 Descripción
Este proyecto es una aplicación web desarrollada en el contexto de una simulación profesional de No Country, cuyo objetivo es construir un CMS (Content Management System) que permita:
- Crear y gestionar testimonios  
- Publicar contenido multimedia (imágenes, videos, etc.)  
- Administrar usuarios y autenticación con JWT  
- Visualizar contenido en una interfaz moderna  

## 🧱 Arquitectura del Proyecto
El proyecto sigue una arquitectura desacoplada basada en microservicios:
📦 root  
 ┣ 📂 backend      → API REST (Spring Boot)  
 ┣ 📂 frontend     → Aplicación web (Vite / Node.js)  
 ┣ 📄 docker-compose.yml  
 ┗ 📄 README.md  
  
## 🛠️ Tecnologías utilizadas
> Backend
> + Java 21  
> + Spring Boot  
> + Spring Security  
> + JWT (JSON Web Tokens)  

> Frontend
- Node.js 22+
- Vite  
- JavaScript / (posible React)  

> DevOps
- Docker  
- Docker Compose  

## ⚙️ Requisitos
Antes de ejecutar el proyecto, asegúrate de tener instalado:
- Node.js 22+  
- Java 21+  
- Docker (opcional pero recomendado)

## 🚀 Ejecución del proyecto
🔹 Opción 1: Desarrollo local
> Backend
- cd backend  
./mvnw spring-boot:run
Frontend
cd frontend
npm install
npm run dev
🔹 Opción 2: Docker (Recomendado)
docker-compose up --build

📍 Accesos:

Frontend → http://localhost:5173
Backend → http://localhost:8080
🔐 Variables de entorno

⚠️ Este proyecto requiere archivos .env para su correcto funcionamiento.

📁 Backend (backend/.env)

Ejemplo:

SPRING_DATASOURCE_URL=jdbc:postgresql://db:5432/testdb
SPRING_DATASOURCE_USERNAME=postgres
SPRING_DATASOURCE_PASSWORD=postgres

JWT_SECRET=1234567890abcdef1234567890abcdef
JWT_EXPIRATION=3600000
📁 Frontend (frontend/.env)
VITE_API_URL=http://localhost:8080
🔒 Seguridad (JWT)

El sistema utiliza autenticación basada en JWT.

⚠️ IMPORTANTE:

La clave JWT_SECRET debe tener un mínimo de 256 bits (32 caracteres).
Claves más cortas generarán errores de seguridad en la aplicación.
🐳 Docker

Este proyecto incluye un archivo docker-compose.yml que permite levantar todos los servicios de forma sencilla.

Comandos útiles:
# Construir y levantar contenedores
docker-compose up --build

# Detener contenedores
docker-compose down
🤝 Contribución

Proyecto desarrollado en equipo bajo metodología ágil (Scrum) en el entorno de No Country.

Si deseas contribuir:

Fork del repositorio
Crear una nueva rama
Realizar cambios
Crear Pull Request
📌 Estado del proyecto

🚧 En desarrollo

👨‍💻 Autor / Equipo

Equipo 06 - No Country Simulation
Participantes del proyecto colaborativo

📄 Licencia

Este proyecto es de uso educativo dentro del programa No Country.
