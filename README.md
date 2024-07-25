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
docker compose build

# 5. Iniciar os Containers Docker
docker compose up -d

# 6. Executar as Migrações do Banco de Dados
docker exec -it web php artisan migrate

# 7. Popular o Banco de Dados
docker exec -it web php artisan db:seed

# 8. Acessar a Aplicação
# Abra seu navegador e acesse o endereço:
# http://localhost:8080/
