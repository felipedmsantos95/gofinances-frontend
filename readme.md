# GoFinances Frontend

<p align="center">
    <a href="readme_en.md">English</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
    <a href="readme.md">Português</a>&nbsp;&nbsp;&nbsp;
</p>

## Prévia da Aplicação

<p align="center">
  <img src="https://github.com/felipedmsantos95/gofinances-frontend/blob/master/src/assets/gofinances.gif"/>
</p>

## Sobre

Plataforma web em React.js para gestão de transações com envio de arquivos por formulário. O repositório do backend está disponível [aqui](https://github.com/felipedmsantos95/gofinances-backend).


## Tecnologias utilizadas

- React.js

## Requisitos

Para executar o projeto é necessário ter os seguintes requisitos instalados no sistema:

- Node 12.x ou superior
- Yarn 1.21 ou superior

## Executando o projeto

### Clonando o projeto

```bash
$ git clone https://github.com/felipedmsantos95/gofinances-frontend
$ cd gofinances-frontend
```

### Scripts para execução do projeto

Dentro do diretório do projeto pela primeira vez, você deve executar o comando `yarn` para instalar as dependências, então será possível rodar os seguintes scripts:

#### `yarn start`

Executa o app em modo de desenvolvimento.<br />
Abra [http://localhost:3000](http://localhost:3000) para ver em um navegador web.

A página irá recarregar quando você fizer edições.<br />
Você poderá visualizar quaisquer erros no console.

#### `yarn test`

Executa o modo teste da aplicação com modo interativo.<br />
Você pode consultar a sessão ["Running tests"](https://facebook.github.io/create-react-app/docs/running-tests) na documentação do React para mais informações.

#### `yarn build`

Compila o app para entrar em modo de produção para a pasta chamada `build`.<br />
Desta forma, isso organiza o React no modo de produção e otimiza a compilação para obter melhor desempenho.

Você pode consultar a sessão ["Deployment"](https://facebook.github.io/create-react-app/docs/deployment) na documentação do React para mais informações.


<h3 align="center">
  Enunciado do desafio proposto
</h3>

## Sobre o desafio

Nesse desafio, você deve continuar desenvolvendo a aplicação de gestão de transações, a GoFinances. Agora você irá praticar o que você aprendeu até agora no React.js junto com TypeScript, utilizando rotas e envio de arquivos por formulário.

Essa será uma aplicação que irá se conectar ao seu backend do [Desafio 06](https://github.com/felipedmsantos95/gofinances-backend), e exibir as transações criadas e permitir a importação de um arquivo CSV para gerar novos registros no banco de dados.


### Funcionalidades da aplicação


- **`Listar as transações da sua API`**: Sua página `Dashboard` deve ser capaz de exibir uma listagem através de uma tabela, com o campo `title`, `value`, `type` e `category` de todas as transações que estão cadastradas na sua API.

- **`Exibir o balance da sua API`**: Sua página `Dashboard`, você deve exibir o balance que é retornado do seu backend, contendo o total geral, junto ao total de entradas e saídas.

- **`Importar arquivos CSV`**: Na sua página `Import`, você deve permitir o envio de um arquivo no formato `csv` para o seu backend, que irá fazer a importação das transações para o seu banco de dados. O arquivo csv deve seguir o seguinte [modelo](https://github.com/Rocketseat/bootcamp-gostack-desafios/blob/master/desafio-database-upload/assets/file.csv).



### Específicação dos testes

Para esse desafio temos os seguintes testes:

- **`should be able to list the total balance inside the cards`**: Para que esse teste passe, sua aplicação deve permitir que seja exibido na sua Dashboard, cards contendo o total de `income`, `outcome` e o total da subtração de `income - outcome` que são retornados pelo balance do seu backend.

* **`should be able to list the transactions`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados dentro de uma tabela, toda as transações que são retornadas do seu backend.

- **`should be able to navigate to the import page`**: Para que esse teste passe, você deve permitir a troca de página através do Header, pelo botão que contém o nome `Importar`.

- **`should be able to upload a file`**: Para que esse teste passe, você deve permitir que um arquivo seja enviado através do componente de drag-n-drop na página de `import`, e que seja possível exibir o nome do arquivo enviado para o input.
