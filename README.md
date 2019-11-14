# Problema
Atualmente o Cartão de Todos tem 2,5 milhões de famílias ativas e uma das formas de recebimento é o cartão de crédito, um dos problemas dessa forma de cobrança é o vencimento dos cartões, por isso surge um problema de criar um uma busca rápida para antecipar esses vencimentos e conseguirmos colocar uma nova forma de cobrança.

# Escopo
Implemente uma API REST para realizar uma busca de cartões que irão vencer
em um determinado mês e ano.

O desafio é composto de duas partes:
  1. Sistema, onde você precisa criar uma estrutura de cadastro do cliente e seus cartões relacionados e implementar um algoritmo que, dado a estrutura de dados acima e uma query, retornará com o conjunto de cartões que possuem o vencimento do cartão para um mês/ano especifico.
  2. Uma API REST (Você pode utilizar qualquer biblioteca que quiser) que recebe uma query, faz uma busca no sistema de utilizando o algoritmo e retorna os cartões ativos que irão vencer em um determinado mês/ano.
  
Exemplo de um endpoint para a API REST:
```
curl -X GET -H "Content-Type: application/json" http://localhost:8000/valid-
thru/?month=02&year=2020
```

Resposta:
```
[{
  'client_id': 22,
  'card_holder': 'Roberto Justus',
  'card_number': '**********9374',
  'month': 02,
  'year': 2020,
  'is_active': true
},
{
  'client_id': 22,
  'card_holder': 'Luciano Huck,
  'card_number': '**********3649,
  'month': 02,
  'year': 2020,
  'is_active': true
}, ...
]
```

# O que esperamos
  - Que o desafio seja feito em Python 3+
  - Que tenha testes automatizados.
  - Que você implemente a API REST para que, dado uma query, retorne os possíveis cartões.
  - Que seja fácil de rodarmos seu desafio em um ambiente Linux.
  - Crie um dataset cards.csv para popular a base com dados fictícios.
  - Que você popule a Estrutura de Dados quando a API REST inicializar, em memória.
  - Deixe o código em inglês
  - Use Git
  - Procure fazer micro commits que são muitos commits com menos código isso nos ajuda a compreender a sua lógica
  - Nos pergunte sobre qualquer dúvida que venha a surgir durante o desenvolvimento
  - Documente detalhadamente quaisquer referencias/ferramentas que vc pesquisar
  - Crie um repositório público e nos passe o link para acompanharmos o desenvolvimento
