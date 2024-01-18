
#  Loja de Games

Atividade Spring do Bootcamp:

    "Construa o Backend para uma Loja de Games com a capacidade de manipular os dados dos Produtos da loja. Os produtos deverão estar classificados por Categoria."





## Funcionalidades

- Consultas de dados pelo método GET
- Inserção de registros pelo método POST
- Atualização de registros pelo método PUT
- Deleção de registros pelo método DELETE

## Documentação da API 

### Produto

#### Retorna todos os produtos

```
  GET /produto
```

#### Retorna um produto pelo ID

```
  GET /produto/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. O ID do produto que você quer |


#### Retorna um produto pelo nome

```
  GET /produto/nome/${nome}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `nome`      | `string` | **Obrigatório**. O nome do produto que você quer |


#### Registra um produto

```
  POST /produto
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `nome`      | `string` | **Obrigatório**. Nome do produto para registro|
| `descricao`      | `string` | **Obrigatório**. Descrição do produto para registro|
| `preco`      | `string` | **Obrigatório**. Preço do produto para registro|
| `categoria: { id: }`      | `int` | **Obrigatório**. Id da categoria do produto|


#### atualização de um produto pelo ID

```
  PUT /produto
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. Id do produto para atualização|
| `nome`      | `string` | **Obrigatório**. Nome do produto para atualização|
| `descricao`      | `string` | **Obrigatório**. Descrição do produto para atualização|
| `preco`      | `string` | **Obrigatório**. Preço do produto para atualização|
| `categoria: { id: }`      | `int` | **Obrigatório**. Id da categoria do produto para atualização|


#### Deleção de um item pelo ID

```
  DELETE /produto/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. Id do produto para deleção|


### Categoria

#### Retorna todos as categorias

```
  GET /categoria
```

#### Retorna uma categoria pelo ID

```
  GET /categoria/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. O ID da categoria que você quer |


#### Retorna uma categoria pelo nome

```
  GET /categoria/nome/${nome}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `nome`      | `string` | **Obrigatório**. O nome da categoria que você quer |


#### Registra uma categoria

```
  POST /categoria
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `nome`      | `string` | **Obrigatório**. Nome da categoria para registro|
| `descricao`      | `string` | **Obrigatório**. Descrição da categoria para registro|


#### atualização de uma categoria pelo ID

```
  PUT /categoria
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. Id da categoria para atualização|
| `nome`      | `string` | **Obrigatório**. Nome da categoria para atualização|
| `descricao`      | `string` | **Obrigatório**. Descrição da categoria para atualização|


#### Deleção de uma categoria pelo ID

```
  DELETE /categoria/${id}
```

| Parâmetro   | Tipo       | Descrição                                   |
| :---------- | :--------- | :------------------------------------------ |
| `id`      | `string` | **Obrigatório**. Id da categoria para deleção|

## Stack utilizada

**Back-end:** Java, Spring Boot, MySQl

**Testes:** Insomnia


## Processo de desenvolvimento das branches

Main 

- Inicialização do projeto Spring 
- Configuração da application.properties para conexão com o banco de dados 
- Criação das camadas Repository, Model, e Controller.

RelacionamentoTabelas 

- Desenvolvimento das classes Produto e Categoria com os seus devidos atributos  
- Annotations
- Relacionamento OneToMany e ManyToOne entre elas.

Crud 

- Conexão com o JpaRepository
- Dois métodos personalizados
- Autowired para injeção de dependências
- Desenvolvimento dos métodos HTTP (GET, POST, PUT e DELETE).

**Antes de enviar a atividade, realizei os testes no Insomnia juntamente com o MySQL para ver se tudo estava funcionando e fiz o merge para a main.**

## Aprendizados

Essa parte prática me ajudou muito na fixação dos conteudos passados em aula e das leituras feitas em cima da documentação do bootcamp. Senti mais confiança no desenvolvimento dessa tarefa e sinto que a cada prática realizada isso tende a crescer.




