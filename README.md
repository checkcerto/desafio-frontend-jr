# Desafio Font-end Jr. AutoSCORE

## Avisos antes de começar
- Crie um repositório publico no seu GitHub *sem citar nada* relacionado a AutoSCORE ou CheckCerto.
- Faça seus commits no seu repositório.
- Você poderá consultar o Google, Stackoverflow ou algum projeto particular na sua máquina.

### Sobre o ambiente da aplicação:
- A linguagem de programação escolhida é Typescript;
- Deve ser usado o Framework Angular 12+;
- Recomendamos o uso da seguinte suite de componentes: PrimeNG;

## Objetivo
Temos o objeto de cadastrar uma pessoa e seu veiculo no sistema, para isso crie um formulário (CRUD), para que seja possivel gerenciar esse cadastro.

### API que será cosumida
Para o teste usaremos a seguinte API *https://my.api.mockaroo.com/cars*, nela estão habilitados os verbos:
- GET / - Retorna todos os registros;
- GET /id - Retorna o registro através do código;
- POST / - Realiza um novo cadastro;
- PUT /id - Atualiza um cadastro através do código;
- PATCH /id - Atualiza o campo first_name através do código;
- DELETE /id - Exclui o registro através do código;

*Exemplo de uso*

POST: (https://my.api.mockaroo.com/cars)

```json
{
    "first_name": "Fulano",
    "last_name": "de Tal",
    "email": "fulano@email.com.br",
    "car_plate": "FAG9B88",
    "car_vin": "5UXWX9C52D0246778",
    "car_make": "Chevrolet",
    "car_model": "Onix 1.4 LTZ",
    "car_model_year": 2019
}
```

* Os campos *first_name*, *last_name*, *email* e *car_plate* serão obrigatórios o preenchimento;
* O campo *plate* poderá apenas receber placas de veiculo, no formato AAA1234 ou AAA1A34.

Para autenticação da transação é preciso usar a seguinte chave *55ad1cd0*, que pode ser passada através de um parametro (key) ou do cabeçalho (header):

Exemplos: 
- Parametro: GET (https://my.api.mockaroo.com/cars/1?key=55ad1cd0)
- Cabeçalho: 
```curl
curl -H "X-API-Key: 55ad1cd0" https://my.api.mockaroo.com/cars/123
```

# Avaliação
Serão avaliados a implementação e consumo da RestAPI, e a UI e UX da aplicação.

## O que será um Diferencial
- Validação dos dados de entrada
- Código limpo e organizado (nomenclatura, etc)
- Modelagem de Dados
- Tratamento de erros
- Uso de Design Patterns

# Materiais úteis (Referencia)
- https://angular.dev
- https://primeng.org
- https://www.dio.me/articles/criando-um-aplicativo-angular-17-para-consumir-apis-um-guia-detalhado
- https://www.youtube.com/watch?v=rjrQpMYtTUw

