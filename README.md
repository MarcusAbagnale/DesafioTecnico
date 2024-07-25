# Projeto de Cadastro de Pessoas com Laravel e Vue

## Requisitos

- Docker instalado e configurado
- Git instalado

## Instruções de Configuração

```bash
# 1. Clonar o Repositório
git clone https://github.com/MarcusAbagnale/DesafioTecnico.git

# 2. Entrar na Pasta do Projeto
cd DesafioTecnico

# 3. Configurar os Arquivos .env
# - Backend: Configure o arquivo `.env` localizado na pasta `app` com as informações adequadas para o backend.
# - Frontend: Configure o arquivo `.env` localizado na pasta `front` com as informações adequadas para o frontend.

# 4. Construir os Containers Docker
**Execute os comandos em terminal Bash**
docker compose build

# 5. Iniciar os Containers Docker
docker compose up -d

# 6. Instalar as dependências
docker exec -it web composer install

# 7. Executar as Migrações do Banco de Dados
docker exec -it web php artisan migrate

# 8. Popular o Banco de Dados
docker exec -it web php artisan db:seed

# 9. Acessar a Aplicação
# Abra seu navegador e acesse o endereço:
# http://localhost:8080/

```
```
git clone https://github.com/MarcusAbagnale/DesafioTecnico.git
cd DesafioTecnico
bash
docker compose build
docker compose up -d
docker exec -it web composer install
docker exec -it web php artisan migrate
docker exec -it web php artisan db:seed```

```
#Diagrama de Relacionamento do Banco de Dados

<img src="https://github.com/user-attachments/assets/e8f42d84-2fe7-4e84-836a-eaec43274cc2">




