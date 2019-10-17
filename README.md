# TDD-NODEJS
Testes em Nodejs

### `docker run --name database2 -e POSTGRES_USER=docker -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres:11`
Cria a máquina virtual do postgres passando como parametro o nome do container no docker, usuário do banco de dados, senha do banco de dados e a porta que irá rodar o banco de dados.

### `docker start database`
Inicia a máquina virtual.

### `git clone https://github.com/victorreinor/tdd-nodejs`
Clona o repositório do projeto.

### `cd tdd-nodejs`
Entra dentro da pasta do repositório.

Em seguida crie um arquivo **.env** com base no **.env.example** para setar as variáveis de configuração do sistema.

Caso a máquina virtual for criada igual a do exemplo acima, não irá precisar alterar nada, somente crie a **.env** copiando o conteúdo completo.

### `yarn sequelize db:migrate`
Roda as migrations para subir as tabelas do banco de dados.

### `yarn install`
Instala as dependências que estão sendo usadas no projeto.

### `yarn dev`
Inicia o projeto.

Em seguida importe o arquivo **insomnia.json** dentro do rest cliente **Insomnia**.

## Comandos adicionais caso necessário

#### `yarn sequelize migration:create --name=`
Cria uma migration e passa como parametro o nome da migration.

#### `docker ps`
Exibe todos os containers que estão onlines.

#### `docker ps -a`
Exibte todos os containers que foram criados.