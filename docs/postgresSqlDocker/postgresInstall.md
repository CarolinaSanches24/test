#### 1 - ATUALIZAR PACOTES

```bash
sudo apt-get update
```

#### 2- Solicitando imagem

```bash
docker pull postgres
```

#### 3 - Listar containers 

```bash
docker ps
```
#### 4- Criar um container docker

```bash
docker run --name ContainerPostgres -e POSTGRES_PASSWORD= -d postgres
```
![alt text](image.png)

#### 5 - Acessando o container

```bash
docker exec -it ContainerPostgres psql -U postgres 
```

#### 6 - Teste de conexão

```bash 
SELECT NOW();
```

#### 7- Sair do postgres

```bash
\q
```
