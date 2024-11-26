# Usa una imagen base de Node.js
FROM node:16

# Define el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia los archivos package.json y package-lock.json para instalar las dependencias
COPY package*.json ./

# Instala las dependencias de la aplicación
RUN npm install

# Copia el resto de los archivos de tu aplicación al contenedor
COPY . .

# Expón el puerto en el que la app estará escuchando (ajústalo si es necesario)
EXPOSE 3000

# Comando para ejecutar la aplicación
CMD ["node", "app.js"]
