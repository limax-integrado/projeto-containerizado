FROM node:20-alpine

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 3000

# O parâmetro --host é necessário para o Vite escutar as conexões do Docker/Nginx
CMD ["npm", "run", "dev", "--", "--host"]