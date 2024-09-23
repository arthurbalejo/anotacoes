[[Banco de Dados]]

### lista todos containers

```
docker -a
```
### para ativar o conteiner
```
docker start <nome>
```
### para verificar se o conteiner está ativado e informações
```
docker ps
```
### para parar o conteiner

```
docker stop <3 primeiras caracteres>
```

### subindo container e definindo match das portas e senha(primeira porta é a minha)
```
 docker run --name mysql -e MYSQL_ROOT_PASSWORD=126310 -p 3306:3306
```

### verificar portas disponiveis no windows
```
netstat -ano | findstr :<número_da_porta>
```
