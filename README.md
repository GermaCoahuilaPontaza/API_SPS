# API_SPS
Prueba para la creación de una API

📡 API de Clientes - MuleSoft
Este proyecto expone una API en MuleSoft para consultar información de clientes desde una base de datos MySQL. Implementa Secure Properties para proteger credenciales y está listo para desplegarse en CloudHub.
📌 Endpoints
Método	GET
Ruta    /api/v1/sps/customers
Descripción Obtiene la lista de clientes desde la base de datos

🛠 Instalación y Configuración
🔹 1. Clonar el repositorio
Ejecuta el siguiente comando en tu terminal:
git clone https://German Coahuila Pontaza/API_SPS.git

🔹 2. Importar en Anypoint Studio
Abre Anypoint Studio.
Selecciona File > Import > Anypoint Studio Project from File System.
Selecciona la carpeta del proyecto clonado.
🔹 3. Configurar propiedades del entorno
En la carpeta src/main/resources/config/ se encuentran los archivos de configuración:
📄 local.properties (para pruebas locales):
📄 dev.properties (para desarrollo):
📄 local.properties.secure (credenciales cifradas):

Nota: Cifrar estas credenciales con mule-secure-properties-tool.

🚀 Ejecución y Pruebas
🔸 Ejecutar la API en Anypoint Studio
Click derecho en el proyecto → Run As > Mule Application
La API estará disponible en http://localhost:8081/api/v1/sps/customers
🔸 Probar la API con Postman
GET http://localhost:8081/api/v1/sps/customers
Debe retornar un JSON con la lista de clientes.
Ejemplo de respuesta:

[
    {
        "FirstName": "Maura",
        "LastName": "Wagstaffe",
        "Email": "mwagstaffe@npr.org",
        "Company": "Kazu"
    },
    {
        "FirstName": "Myrwyn",
        "LastName": "Eliet",
        "Email": "meliet1@buzzfeed.com",
        "Company": "Skibox"
    }
]


☁ Despliegue en CloudHub
Para desplegar la API en CloudHub, sigue estos pasos:

Accede a Anypoint Platform → Runtime Manager
Click en Deploy Application
Configura:
Application Name: api-customers
Worker Size: 0.1 vCores (para pruebas)
Properties: Cargar los archivos de configuración.
Click en Deploy

La API estará disponible en:
https://api-customers.cloudhub.io/api/v1/sps/customers

📌 Tecnologías Utilizadas
✔ MuleSoft 4
✔ Anypoint Studio
✔ MySQL
✔ CloudHub

✨ Autor
📌 [German Coahuila Pontaza]
📧 Contacto: [ger_9321@gmail.com]
