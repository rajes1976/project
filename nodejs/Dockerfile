# Gebruik het officiële Node.js Docker image
FROM node:23

# Stel de werkdirectory in
#WORKDIR /nodejs
WORKDIR /usr/src/app

# Kopieer package.json en package-lock.json
COPY /nodejs/ .
#COPY . .

# Installeer de vereiste pakketten
RUN npm install

# Bundle app source
COPY . .

# Exposeer de poort waarop de app draait
EXPOSE 3000

# Voer de applicatie uit
CMD ["node", "app.js"]
