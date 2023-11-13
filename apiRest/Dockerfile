# Utiliza la imagen oficial de Node.js 18 basada en Alpine Linux
FROM node:latest

# Establece el directorio de trabajo dentro del contenedorr
WORKDIR /app

# Copia el package.json y package-lock.json al directorio de trabajo
COPY package*.json ./

# Instala las dependencias de las aplicaciones
RUN npm install

# Copia el resto de los archivos de la aplicación al directorio de trabajo.
COPY . .

# Expone el puerto en el que se ejecutará la aplicación.
EXPOSE 3000

# Comando para ejecutar la aplicación cuando se inicia el contenedor
CMD ["node", "index.js"]
