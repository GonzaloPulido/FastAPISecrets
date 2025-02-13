# Guía para ejecutar el proyecto 

Sigue estos pasos para desplegar la API de manera sencilla con Docker.  

## 1️⃣ Clonar el repositorio  
Abre una terminal y ejecuta el siguiente comando para clonar el proyecto en tu máquina:  

bash
git clone https://github.com/GonzaloPulido/FastAPISecrets.git


## 2️⃣ Acceder a la carpeta del proyecto  
Navega hasta la carpeta que contiene el código clonado:  

bash
cd FastAPISecrets


## 3️⃣ Configurar variables de entorno  
El proyecto usa un archivo .env para definir configuraciones sensibles. Renombra el archivo de ejemplo:  

bash
mv .env_javi .env


## 4️⃣ Construir la imagen de Docker  
Ejecuta el siguiente comando para construir la imagen del contenedor:  

bash
docker build -t mi-api-segura .


## 5️⃣ Ejecutar el contenedor  
Inicia el contenedor en segundo plano y mapea el puerto 8000:  

bash
docker run -d -p 8000:8000 mi-api-segura


## 6️⃣ Probar la API  
Accede a la API en tu navegador o con curl:  

🔹 *Consulta de usuarios:*  
👉 [http://localhost:8000/users](http://localhost:8000/users)
