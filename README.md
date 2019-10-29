# tdd-js

O que é tdd ? **Test-driven development** (Desenvolvido dirigido a testes), serve para:
- Criar testes antes das funcionalidades
  - É desenvolvido um teste de função especifica antes mesmo de ela existir, assim auxiliando no desenvolvimento pois já sabemos o que nos espera no final.
- Facilita visualização das regras de negócio
  - Geralmente definimos os testes, o comportamento dele e o que esperamos dele, e ai depois fazemos a aplicação funcionar

Code Covarage:
- Coleta informações das linhas de códigos que seus testes atuais não alcançaram;
  - Exibe as linhas que ainda não foram testadas e retorna atraves de uma interface gráfica e o percentual de cada controller testado.

Por que testar ?
- Garantir que tudo vai continuar funcionando;

Tipos de testes
- Testes Unitários
  - Testa uma função mínima e pura, que não realiza efeitos colaterais como acessos ao banco ou integrações externas;
- Testes de Integração
  - Os principais testes do back-end, testam funcionalidades completas como acesso à rotas até retorno do controller;
- Testes E2E
  - Testes de interface que simulam o acesso do usuário (front-end);

Ferramenta que será utilizada:
- **Jest**: Desenvolvido pelo Facebook para testes, funciona no Nodejs, React, React-Native. Ele contém tudo o que precisa em conceito de testes e não precisa ficar instalando dependências a parte para suprir a demanda.

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
