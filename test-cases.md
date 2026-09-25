# Casos de Teste — SauceDemo

Documentação dos testes manuais realizados na aplicação SauceDemo.

## CT-001 - Adicionar produto ao carrinho

### Objeitvo
Verificar se o usuário consegue adicionar um produto ao carrinho corretamente.

### Pré-condições
- Usuário autenticado na aplicação.
- Usuário na página de produtos.

### Passos
1. Localizar o produto Sauce Labs Backpack.
2. Clicar no botão "add to cart".
3. Acessar o carrinho.
4. Verificar se o produto foi adicionado.

### Resultado esperado
O produto deve ser adicionado ao carrinho, apresentando quantidade 1 e preço $29.99.

### Resultado obtido 
O produto foi adicionado corretamente. O botão "add to cart" mudou para "Remove". O produto apareceu no carrinho com quantidade 1 e preço $29.99.

### Status
**PASSOU**


## CT-002 - Adicionar múltiplas unidades do mesmo produto

### Objetivo
Verificar se o usuário consegue adicionar mais de uma unidade do mesmo produto ao carrinho.

### Pré-condições 
- Usuário autenticado na aplicação.
- Produto Sauce Labs Backpack disponível.

### Passos
1. Adicionar o produto Sauce Labs Backpack ao carrinho.
2. Retornar á página de produtos.
3. Tentar adicionar novamente o mesmo produto.
4. Acessar o carrinho.
5. Verificar se existe uma opção para aumentar a quantidade do produto.

### Resultado esperado
O sistema deve permitir ao usuário adicionar mais de uma unidade do mesmo produto ou disponibilizar uma opção para alterar sua quantidade no carrinho.

### Resultado obtido
Após adicionar o produto, o botão passou de "Add to cart" para "Remove", não sendo possível adicionar uma segunda unidade pela página de produtos.
No carrinho também não foi encontrada uma opção para aumentar a quantidade do produto.

### Status
**OBSERVAÇÃO FUNCIONAL**
