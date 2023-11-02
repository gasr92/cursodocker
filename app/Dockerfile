FROM node:12-alpine
WORKDIR /app
# RUN addgroup dev && adduser -S -G gabriel dev
# #&& executa comandos em sequencia

# USER gabriel

COPY package.json .
RUN apk add --no-cache python2 g++ make
RUN yarn install --production

COPY . .

CMD ["node", "src/index.js"]
#run executa enquanto a imagem esta sendo construida
#cmd executa quando a imagem já esta rodando (ja foi construida)


EXPOSE 3000

#ADD http:www.site.com/arquivoteste.json
#ADD teste.zip - o metodo add ja descompacta o zip