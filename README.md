# API-descomplicada
Um guia de como usar API

Fala gafanhotooo, se você está começando na programação ou se esse nome API te deixa calafrios, então dá uma segurada aí e vamos lá aprender esse treco rs.

### O que é API 
API (Application Programming Interface) nada mais é do que uma URL onde é possível consumir dados e integrar sistemas. Na maioria das vezes os dados vem via **JSON (significa JavaScript Object Notation)** que é um formato de transferência de dados.
Agora que você já sabe disso vamos partir para a prática.

### Modo tradicional x Frameworks
Vamos fazer um comparativo de qual o melhor jeito de consumir APIs usando o método tradicional vs os frameWorks

##### XMLHttpRequest
Esse carinha estranho que vamos usar para fazer o nosso request da API
```
let xhr = new XMLHttpRequest();

xhr.open(method, URL, [async, user, password])

xhr.send([body])
```
traduzindo esse pequeno pedaço de código 
***let xhr = new XMLHttpRequest();*** 
aqui você está armazenando o seu request em uma variável
***xhr.open(method, URL, [async, user, password])*** Nesee pedaço de código está acontecendo algumas coisinhas se liga
* xhr.open - como o nome já fala, é o método que vai "abrir" a api 
* method - aqui nós temos duas opções de enviar nosso request, pode ser via **POST** ou **GET**, vamos para uma explicação rápida 
####### POST 
É uma requisição encapsulada na URL, então quando o request é feito você não ve o contéudo pepla url diferente do GET
####### GET 
É a requisição onde os dados não são encapsuladas exemplo
**/logar?email=turan-98%mail.com&senha=batman123** viu toda a informação fica visivel na url, não é uma boa opção para senhas kkk
* URL - é a url da api
* password - algumas APIs pedem o acesso e aqui você vai colocar o login e usuário que ela der 
* xhr.send - aqui nós enviamos o nosso request :0 


