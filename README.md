# Descrição do teste - Front-end

## 1. Especificação
	
O teste consiste em consumir uma API e realizar as tarefas solicitadas.

*Para a criação da API foi utilizado o [json server](https://github.com/typicode/json-server).*

## 2. Tarefas

### 2.1 Listar usuários

endpoint:
 ```
 https://front-test-pg.herokuapp.com/users
 ```

**Quando** o usuário acessar a home
**Então** deve ser exibida a lista de usuários

*********

| id | avatar | name | age | count_messages |
|----|--------|-----|------|----------------|
| 3552 | _imagem_ | José do Boné | 56 | 23 |
| 2534 | _imagem_ | Mariazinha   | 31 | 86 |
*********

**Desejável**

1. Busca por nome;
2. Ordenar tabela pelo campo;

### 2.2 Mensagens enviadas

endpoint:
 ```
 https://front-test-pg.herokuapp.com/messages
 ```

**Quando** clicar no usuário
**Então** deve ser exibida a lista de mensagens enviadas ao usuário

*********
Name: José do Boné

Total: 23

| id | type | contact | date_schedule | date_send | status |
|----|------|---------|--------|--------|--------|
| 121 | EMAIL| jose@bone.com | 2019-02-06 08:53 | 2019-02-06 08:54 | NOT_DELIVERED |
| 123 | SMS  | 41877552369 | 2019-02-07 08:15 | 2019-02-07 08:25 | NOT_DELIVERED |
| **3121** | **EMAIL** | **jose@bone.com** | **2019-02-08 17:53** | **2019-02-08 18:51** | **DELIVERED** |
| 3431 | SMS| 41877552369 | 2019-02-10 08:36 | 2019-02-10 08:37 | NOT_DELIVERED |

*********

**Desejável:**
1. Filtro por tipo;
2. Filtro por status;
3. Filtro por mês;
4. Paginação;
5. Ordenar tabela pelo campo;
6. Assinalar quando a diferença entre a data de envio(sended) e a data de agendamento(scheduled) for superior a 30 minutos;

## Requisitos do projeto
* Fornecer os códigos fonte para avaliação enviando o link do seu github, gitlab, bitbucket ou codepen;
* Escreva a documentação do projeto contendo: 
	* Descrição;
	* Instruções de como instalar e testar;
	* Breve descrição de como foi desenvolvido (sistema operacional, editor de texto/IDE, bibliotecas, etc).
* Variáveis, código e strings devem estar todos em inglês.

## Recomendações
* Vue.js
* Nuxt.js
* Sass 
* Bootstrap 4
* Internacionalização
* webpack / gulp / grunt
* npm / bower

## O que será avaliado?
* Boa lógica de programação ([Clean code](https://de.wikipedia.org/wiki/Clean_Code))
* Boas práticas de UX
* Criatividade
* Vanilla javascript
* CSS3 / HTML5 / Sass
* Boas práticas do git
* Desenvolvimento de sites responsivos
* Quantidade de itens desejáveis realizados