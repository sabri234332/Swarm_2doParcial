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
EXPOSE 4000

# Command to run the application when the container starts
CMD ["node", "index.js"]
