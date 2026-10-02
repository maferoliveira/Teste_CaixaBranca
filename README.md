# Teste de Caixa Branca

Atividade da disciplina de **Testes de Software**, do curso de Desenvolvimento de Sistemas.

## Sobre a atividade

Nesta atividade foi analisado um sistema de pedidos feito em **HTML, CSS e JavaScript**.

O sistema permite escolher um produto, informar a quantidade, usar um cupom de desconto, escolher o tipo de frete e calcular o valor final do pedido.

O objetivo foi analisar o código por dentro e encontrar **seis erros de lógica**, criando testes para mostrar o comportamento incorreto de cada um.

## O que foi analisado

Durante a análise foram verificadas principalmente:

* Condições `if`
* Operadores de comparação
* Valores-limite
* Verificação de estoque
* Cupons de desconto
* Frete
* Descontos por quantidade
* Desconto para pedidos de alto valor

## Erros encontrados

Foram encontrados seis erros:

1. **Validação da quantidade** — a quantidade `0` era aceita.
2. **Verificação do estoque** — o sistema não permitia comprar exatamente a quantidade disponível.
3. **Cupom SENAI20** — o desconto era aplicado também com subtotal exatamente igual a R$ 1.000,00.
4. **Frete grátis** — o frete ficava grátis com subtotal exatamente igual a R$ 500,00.
5. **Desconto por quantidade** — o desconto não era aplicado para exatamente 5 unidades.
6. **Pedido de alto valor** — o desconto não era aplicado quando o total era exatamente R$ 3.000,00.

## Testes

Para cada erro foi criado um caso de teste com:

* Dados utilizados;
* Caminho percorrido pelo código;
* Resultado esperado;
* Resultado apresentado;
* Explicação do erro;
* Correção;
* Novo teste após a correção.

Também foram utilizados valores-limite para verificar as condições do sistema.

## Resultado

Depois de identificar os erros, as condições do código foram corrigidas e os mesmos testes foram realizados novamente para verificar se os resultados estavam de acordo com o esperado.

## Tecnologias utilizadas

* HTML
* CSS
* JavaScript

## Autora

**Maria Fernanda M. de Oliveira**
Desenvolvimento de Sistemas — SENAI
