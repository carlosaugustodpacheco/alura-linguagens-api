<h1 align="center">Projeto Alura - Linguagens API</h1>
<h4 align="center"> 
	Projeto raíz funcional finalizado durante a Imersão Java da Plataforma Alura, possibilidade de melhorias de segmentação no futuro. 🚀
</h4>

### 💻 Sobre o projeto

Projeto Back-end Springboot que busca informações no banco de dados MongoDB e disponibiliza na Web no formato JSON na nuvem Heroku ou localmente.
Esse projeto foi desenvolvido em conjunto com o repositório [alura-stickers](https://github.com/carlosaugustodpacheco/alura-stickers) durante a Imersão Java da Plataforma Alura!


### 🎨 Layout

Disponibilizado no Heroku pelo link: https://carlos-alura-linguagens-api.herokuapp.com/linguagens
![image](https://user-images.githubusercontent.com/68930974/181102510-0d4aed1a-1adf-4687-84b8-07f69ed3ebd8.png)

### 👌 Pré-requisitos

Antes de começar, você vai precisar ter instalado em sua máquina o [Git](https://git-scm.com) e um bom editor para trabalhar com o código, nesse projeto utilizei o [VS-Code](https://code.visualstudio.com/).

É necessario também a instalação do JDK 17 e do Maven. Caso utilize o VS-Code é possivel instalar sua extensão facilitada < [Java Extension](https://code.visualstudio.com/docs/java/extensions) >

O repositório [alura-stickers](https://github.com/carlosaugustodpacheco/alura-stickers) que é responsavel pela criação das figurinhas, não é necessario caso a necessidade seja apenas a tratativa do banco de dados e subida para Cloud.

### 🎲 Rodando a aplicação

#### Clone este repositório
```
$ git clone <https://github.com/carlosaugustodpacheco/alura-linguagens-api>
```
#### Acesso
Após carregar todos os arquivos da API, acesse a pasta src\main\java\br\com\alura\linguagensapi do projeto dentro do editor.

#### Execução
Execute o LinguagensApiApplication.java, será iniciado o Springboot em http://localhost:8080/linguagens

#### Alterando banco de dados
Caso queira, é possivel alterar o banco de dados MongoDB, para isso é necessario criar uma conta pelo site do MongoDB e seguir os passos para fazer a conexão da [documentação](https://www.mongodb.com/docs/atlas/connect-to-database-deployment/#connect-to-a-cluster), após isso alterar a chave de acesso gerado no caminho: src\main\resources\application.properties

#### Populando e consultando o banco de dados de imagens localmente
Com o Postman é possivel popular e consultar o banco de dados MonboDB disponibilizado no Heroku.

Para consulta:
```
GET > http://localhost:8080/linguagens
```
Para popular:
```
POST > http://localhost:8080/linguagens
```
Com parametros no "Body" como exemplo abaixo:
```
{
        "title": "Python",
        "image": "https://images.pling.com/img/00/00/08/01/07/1107980/66411-1.png",
        "ranking": 5
    }
```

#### Subindo para Cloud Heroku
Para subir para o Heroku é necessario ter uma conta ativa no [Heroku](https://dashboard.heroku.com/apps) e instalar em sua maquina, no terminal dentro da pasta do projeto:
```
npm install -g heroku
```
Fazer os procedimentos de logar e adicionar a pasta do projeto
```
heroku login
```
```
heroku git:remote -a carlos-alura-linguagens-api
```
Fazer os procedimentos de adicionar, commitar e push do projeto. Após o push será gerado em sua conta um link com o projeto na Cloud.
```
git add -A
```
```
git commit -m
```
```
git push heroku
```

#### Criação de figurinhas
Caso queira gerar figurinhas a partir do JSON da Web (local ou Heroku), seguir passos do repósitorio [alura-stickers](https://github.com/carlosaugustodpacheco/alura-stickers). Fazendo a alteração do link da String no campo 17 da src/App.js para o novo gerado.

### 🛠 Tecnologias

As seguintes ferramentas foram usadas na construção do projeto:

- Java
- Springboot
- MongoDB
- Heroku
- Postman

### ✨ Autor
<a href="https://github.com/carlosaugustodpacheco">
 <img style="border-radius: 50%;" src="https://user-images.githubusercontent.com/68930974/181088945-0a13c969-27ee-46b0-86ee-123d7dea7a89.png" width="150px;" alt=""/>
 <br />
 <sub><b>Carlos Augusto Duru Pacheco</b></sub></a> <a href="https://github.com/carlosaugustodpacheco" title="Rocketseat">🚀</a>
 
  Entre em contato! 👋
  
 [![Linkedin Badge](https://img.shields.io/badge/-Carlos-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/carlosaugustodpacheco/)](https://www.linkedin.com/in/carlosaugustodpacheco/) 
[![Gmail Badge](https://img.shields.io/badge/-carlosaugustodpacheco@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:carlosaugustodpacheco@gmail.com)](mailto:carlosaugustodpacheco@gmail.com)

