![Logo GoStack 12](https://i.imgur.com/UuhPCqe.png)

<h1 align="center">
 Conceitos do NodeJS
</h1>

<div align="center">
 "Ao infinito e além :rocket:"
</div>

## Sobre 🤓

Esse repositório é um desafio apresentado em um curso de NodeJS + Express, a ideia seria criar uma API Rest usando conceitos básicos sobre rotas, middlewares, códigos HTTP, métodos HTTP e por ai vai.

## Funcionamento 🚀💣

 Nossa aplicação é uma API Rest para repositórios, igual ao próprio Github, onde podemos *listar*, *criar*, *atualizar*, *deletar* e *votar* em um determinado repositório.

Temos os métodos:

- **GET**: http://localhost:3333/repositories

    Será responsável por trazer uma lista de repositórios.

- **POST**: http://localhost:3333/repositories

    Essa rota server para criação de um repositório de um repositório e para isso precisamos passar no corpo da requisição algumas informações, segue o exemplo:

    ```json
    {
    	"title": "Desafio II",
    	"url": "http://github.com/desafio-02",
    	"techs":[
    		"NodeJS",
    		"Express"
    	]
    }
    ```

- **PUT**: http://localhost:3333/repositories/:id

    Essa rota server para atualização de um repositório de um repositório, o **:id** deve ser substituído pelo identificador de algum repositório e por fim passamos, no corpo da requisição, as informações que queremos atualizar, segue o exemplo:

    ```json
    {
    	"title": "Desafio IV",
    	"url": "http://github.com/desafio-04",
    	"techs":[
    		"TypeORM",
    		"React Native"
    	]
    }
    ```

- **DELETE**: http://localhost:3333/repositories/:id

    Essa rota server para exclusão de um repositório de um repositório, o **:id** deve ser substituído pelo identificador de algum repositório.

- **POST**: http://localhost:3333/repositories/:id/like

    Com essa rota você pode basicamente dá um like e um determinado repositório, então toda vez que ela é chamada e aumentado o número de likes.

    Para as rotas **POST** e **PUT** o retorno é um objeto, segue exemplo:

    ```json
    {
    	"id": "1a17d8ae-647d-446f-9a84-0561fb9cd28c",
    	"title": "Desafio IV",
    	"url": "http://github.com/desafio-04",
    	"techs":[
    		"TypeORM",
    		"React Native"
    	],
    	"likes": 1
    }
    ```

    **Observação:** A retorno da rota **GET** é basicamente a mesma estrutura só que um invês de ser um objeto é um array de objetos. 

## Como posso usar sua API 🔧🆙 ?

### Requisitos:

- [ ]  [NodeJS](https://nodejs.org/en/)
- [ ]  [Yarn](https://yarnpkg.com/)
- [ ]  [Insomnia](https://insomnia.rest/download/) ou qualquer outra ferramente para teste de API Rest

&nbsp;


___Observação: Vou assumir que você esteja usando Linux 😛.___


&nbsp;

No seu terminal faça um clone do projeto

```bash
git clone https://github.com/brunoJSX/node-concepts-challenge
```

Entre na pasta e dê o comando

```bash
yarn
```

Em seguida basta rodar o comando

```bash
yarn dev
```

E caso tenha um retorno igual a esse:

![https://imgur.com/dotS1tY](https://i.imgur.com/dotS1tY.png)



&nbsp;




**PRONTO** !!! 🚀💥 A API já está funcionando!!!


&nbsp;



Podemos as rotas usando o Insomnia, ou a ferramenta que você escolheu, para fazer os teste, olha um print do meu Insomnia 😻.

- Criando um repositório:

![Insomnia print](https://i.imgur.com/6Zgzq6o.png)

- Buscando os repositórios:

![Insomnia print](https://i.imgur.com/RE1dzhS.png)




&nbsp;
O restante vou deixar por sua curiosidade kkkkk 😝



&nbsp;
<h2 align="center">
 Gostou? 🥳🚀
</h2>

<div align="center">
 Se gostou avalie com uma linda 🌟, dessa forma você irá me incentivar a publicar mais projetos cada vez melhores.
</div>
