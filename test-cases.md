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
3. acessar o carrinho.
4. Verificar se o produto foi adicionado.

### Resultado esperado
O produto deve ser adicionado ao carrinho, apresentando quantidade 1 e preço $29.99.

### Resultado obtido 
O produto foi adicionado corretamente. O botão "add to cart" mudou para "Remove". O produto apareceu no carrinho com quantidade 1 e preço $29.99.

### Status
**PASSOU**
