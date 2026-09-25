# QA testing - SauceDemo
Projeto prático de Quality Assurance realizado com o objetivo de aplicar conceitos de testes de software em uma aplicação web de e-commerce.

## Objetivo
Testar as principais funcionalidades do fluxo de compra da aplicação SauceDemo, verificando o comportamento esperado do sistema, identificando possíveis problemas e documentando os resultados dos testes.

## Escopo dos testes 
Os testes realizados abrangem:
- Login
- Catálogo de produtos
- Remoção de produtos
- Carrinho de compras
- Checkout
- Validação de campos obrigatórios
- Resumo do pedido
- Finalização da compra
- Geração do PDF do pedido

## Resultados 
Foram executados **11 casos de teste**
- 10 casos com resultado **PASSOU**
- 1 caso registrado como **OBSERVAÇÃO FUNCIONAL**
- 0 defeitos confirmados

## Observação funcional
Durante o CT-002 foi observado que a aplicação não disponibiliza uma opção para adicionar múltiplas unidades do mesmo produto ou alterar sua quantidade diretamente no carrinho.
O comportamento foi registrado como observação funcional, sem classificação como defeito, devido à ausência de um requisito que determine essa funcionalidade.

## Documentação 
- [Casos de teste](test-cases.md)

## Ferramentas e conceitos utilizados 
- Testes manuais
- Testes funcionais
- Testes negativos
- Validação de campos
- Análise de comportamento
- Documentação de casos de teste
- GitHub
- Markdown 
