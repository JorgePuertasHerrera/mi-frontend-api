# mi-frontend-api 🚀

Proyecto Full-Stack Serverless desarrollado para aprender y aplicar los fundamentos de la computación en la nube mediante AWS.

## 🏗️ Arquitectura
El proyecto utiliza una arquitectura basada en eventos y servicios gestionados, eliminando la necesidad de gestionar servidores (Serverless).

## 🛠️ Stack Tecnológico
* **Frontend:** HTML5, CSS3, JavaScript.
* **Seguridad:** Amazon Cognito (Gestión de usuarios y autenticación JWT).
* **Backend:** 
  * **API Gateway:** Punto de entrada para las peticiones HTTP.
  * **AWS Lambda:** Lógica de negocio (Serverless functions).
* **Base de Datos:** Amazon DynamoDB (Almacenamiento NoSQL).
* **Infraestructura como Código (IaC):** AWS SAM (Serverless Application Model).

## 💡 ¿Qué hace este proyecto?
Este proyecto implementa un flujo de datos seguro donde el frontend interactúa con una API protegida.
1. El usuario se autentica de forma segura mediante **Cognito**.
2. Una vez autenticado, el frontend realiza peticiones a **API Gateway** con un token JWT.
3. **AWS Lambda** procesa la lógica y realiza operaciones CRUD (Crear, Leer, Actualizar, Borrar) en **DynamoDB**.

## 🚀 Despliegue
Este proyecto utiliza **AWS SAM** para el despliegue de la infraestructura. Para desplegarlo en tu cuenta de AWS, asegúrate de tener instalado el CLI de AWS y SAM:

```bash
sam build
sam deploy --guided
