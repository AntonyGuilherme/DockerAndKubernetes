FROM node

# Todos os comandos serão executados dentro desse diretório
WORKDIR /app

# Copiando o arquivo que informa se houve atualizações nos pacotes utlizados
# para evitar que o npm install seja executado caso qualquer tipo de mudança no código seja feita
# ou seja, esse comando somente será executado se houver mudanças no package.json
COPY package.json /app

# Executando o comando npm install no diretório de trabalho
# Executado quando a imagem é criada
RUN npm install

# Copiando todos os arquivos da raiz para a pasta app
COPY . /app

# Expondo a porta 80 do container, lembrando que por padrão o container é isolado

# Somente para documentação
EXPOSE 80

# Executado quando o container foi inciado
CMD ["node", "server.js"]