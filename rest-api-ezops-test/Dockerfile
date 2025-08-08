# Usa a imagem oficial do Node.js 14
FROM node:14

# Cria diretório de trabalho dentro do container
WORKDIR /app

# Copia os arquivos de dependências
COPY package*.json ./

# Instala as dependências
RUN npm install

# Copia todo o restante do projeto
COPY . .

# Expõe a porta (ajuste se sua API usar outra)
EXPOSE 3000

# Comando para iniciar o servidor
CMD ["node", "server/server.js"]
