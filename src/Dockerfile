ARG TAG=latest
FROM node:$TAG as build
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 8080
CMD ["node", "server.js"]

# FROM alpine:latest as final
# WORKDIR /app
# COPY --from=build /app .
# CMD ["node", "server.js"]

#Não consegui reduzir o tamanho da image, tentei seguir algo parecido que foi demonstrado mais não rolou, se puder dar uma dica eu agradeço.