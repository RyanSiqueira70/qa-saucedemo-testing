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


## CT-003 - Persistência do carrinho após novo login

### Objetivo 
Verificar se o produto adicionado ao carrinho permanece disponível após realizar novo login na aplicação.

### Pré-condições
- Produto Sauce Labs Backpack adicionado ao carrinho.

### Passos
1. Após ser desconectado da aplicação, acessar novamente a página de login. 
2. Realizar login com as credenciais válidas.
3. Acessar o carrinho.
4. Verificar se o produto anteriormente adicionado permanece no carrinho.

### Resultado esperado
O produto adicionado anteriormente deve permanecer no carrinho após o novo login.

### Resultado obtido 
Após realizar um novo login, o produto Sauce Labs Backpack permaneceu no carrinho, mantendo o estado anterior.

### Status
*PASSOU*


## CT-004 - Remover produto do carrinho

### Objetivo
Verificar se o usuário consegue remover um produto do carrinho corretamente 

### Pré-condições 
- Produto Sauce Labs Backpack adicionado ao carrinho.

### Passos
1. Acessar o carrinho.
2. Verificar se o produto Sauce Labs Backpack está presente.
3. Clicar no botão "Remove".
4. Verificar se o carrinho ficou vazio.
5. Retornar à página de produtos.
6. Verificar se o botão do produto voltou para "Add to cart".

### Resultado esperado
O produto deve ser removido do carrinho e o botão na página de produtos deve voltar para "Add to cart", permitindo que o produto seja adicionado novamente.

### Resultado obtido 
Ao clicar em "remove", o produto foi removido corretamente e o carrinho ficou vazio. Ao retornar à página de produtos, o botão voltou para "Add to cart".

### Status
**PASSOU**
