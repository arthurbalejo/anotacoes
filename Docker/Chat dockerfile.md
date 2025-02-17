
```
# Usar uma imagem base do Python
FROM python:3.10

# Definir diretório de trabalho
WORKDIR /app

# Copiar arquivos necessários para dentro do contêiner
COPY . /app

# Ajustar permissões do clidriver (se necessário)
RUN chmod -R 755 /app/clidriver

# Adicionar o clidriver ao PATH
ENV PATH="/app/clidriver/bin:$PATH"

# Instalar dependências
RUN pip install --no-cache-dir -r requirements.txt

# Expor a porta do Flask
EXPOSE 5000

# Comando para rodar a aplicação
CMD ["python", "app.py"]
```

buildar e rodar
```
docker build -t meu_app_flask .
docker run -p 5000:5000 meu_app_flask
```

lembrar de fazer o .dockerignore pra remover o ambiente virtual e o que mais tiver

para salvar a imagem
```
docker save -o meu_app_flask.tar meu_app_flask
```

para carregar em outro computador
```
docker load -i meu_app_flask.tar
```

