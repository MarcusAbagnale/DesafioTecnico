###Projeto de Cadastro de Pessoas com Laravel e Vue
Requisitos
Docker instalado e configurado
Git instalado

###Instruções de Configuração
1. Clonar o Repositório

```git clone <URL_DO_REPOSITORIO>
2. Entrar na Pasta do Projeto

```
cd <NOME_DA_PASTA>
3. Configurar os Arquivos .env
Backend: Configure o arquivo .env localizado na pasta app com as informações adequadas para o backend.
Frontend: Configure o arquivo .env localizado na pasta front com as informações adequadas para o frontend.
4. Construir os Containers Docker
Na pasta raiz do projeto, execute o seguinte comando para construir os containers Docker:

```docker compose build
5. Iniciar os Containers Docker
Ainda na pasta raiz, execute o seguinte comando para iniciar os containers em segundo plano:

```docker compose up -d
6. Executar as Migrações do Banco de Dados
Após os containers estarem em execução, execute o comando abaixo para realizar as migrações do banco de dados:

```docker exec -it web php artisan migrate
7. Popular o Banco de Dados
Execute o comando abaixo para popular o banco de dados com dados de teste:

```docker exec -it web php artisan db:seed
8. Acessar a Aplicação
Abra seu navegador e acesse o endereço:

arduino
Copiar código
http://localhost:8080/

###Considerações Finais
Com esses passos, você terá o ambiente configurado e a aplicação pronta para uso. 
