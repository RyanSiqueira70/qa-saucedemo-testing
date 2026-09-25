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


## CT-005 - Validação dos campos obrigatórios no checkout

### Objetivo 
Verificar se o sistema impede o usuário de prosseguir com o checkout quando os campos obrigatórios não são preenchidos.

### Pré-condições 
- Usuário autenticado na aplicação.
- Produto Sauce Labs Backpack adicionado ao carrinho.

### Passos
1. Acessar o carrinho.
2. Clicar no botão "Checkout".
3. Verificar se a página de informações do checkout é exibida.
4. Não preencher nenhum dos campos obrigatórios.
5. Clicar no botão "Continue".
6. Verificar a mensagem de erro apresentada.

### Resultado esperado
O sistema deve impedir o usuário de prosseguir com o checkout e informar que o campo obrigatório "First Name" precisa ser preenchido.

### Resultado obtido
Ao clicar em "continue" sem preencher os campos, o sistema permaneceu na página de informações do checkout e apresentou a mensagem "Error: First Name is required"

### Status
**PASSOU**


### CT-006 - Validação do campo Last Name

### Objetivo 
Verificar se o sistema impede o usuário de prosseguir quando o campo "Last Name" não é preenchido.

### Pré-condições 
- Usuário autenticado na aplicação.
- Produto Sauce Labs Backpack adicionado ao carrinho.
- Usuário na página de informações do checkout.

### Passos 
1.  Preencher o campo "First Name" com "Ryan".
2. Deixar o campo "Last Name" vazio.
3. Deixar o campo "Zip/Postal Code" vazio.
4. Clicar no botão "Continue"
5. Verificar a mensagem de erro apresentado.

### Resultado esperado
O sistema deve impedir o usuário de prosseguir e informar que o campo "Last Name" é obrigatório.

### Resultado obtido
Após preencher somente o campo "First Name" e clicar em "Continue", o sistema permaneceu na página de checkout e apresentou a mensagem "Error: Last Name is required".

### Status
**PASSOU**


## CT-007 - Validação do campo Zip/Postal Code

### Objetivo 
Verificar se o sistema impede o usuário de prosseguir quando o campo "Zip/Postal Code" não é preenchido.

### Pré-condições 
- Usuário autenticado na aplicação.
- Produto Sauce Labs Backpack adicionado ao carrinho.
- Usuário na página de informações do checkout.

### Passos
1. Preencher o campo "First Name" com "Ryan".
2. Preencher o campo "Last Name" com "Siqueira".
3. Deixar o campo "Zip/Postal Code" vazio.
4. Clicar no botão "Continue".
5. Verificar a mensagem de erro apresentada.

### Resultado esperado
O sistema deve impedir o usuário de prosseguir e informar que o campo "Postal Code" é obrigatório.

### Resultado obtido
Após preencher os campos "First Name" e "Last Name" e clicar em "Continue", o sistema permaneceu na página de checkout e apresentou a mensagem "Error: Postal Code is required".

### Status
**PASSOU**


## CT-008 - Checkout com dados válidos 

### Objetivo
Verificar se o usuário consegue avançar no checkout após preencher corretamente todos os campos obrigatórios e se as informações do pedido são apresentadas corretamente.

### Pré-condições 
- Usuário autenticado na aplicação.
- Produto  Sauce Labs Backpack adicionado ao carrinho.
- Usuário na página de informações do checkout.

### Passos
1. Preencher o campo "First Name" com "Ryan".
2. Preencher o campo "Last Name" com "Siqueira".
3. Preencher o campo "Zip/Postal Code" com "16310000".
4. Clicar no botão "Continue". 
5. Verificar as informações do pedido.
6. Conferir a quantidade do produto.
7. Conferir o preço do produto.
8. Conferir o valor da taxa.
9. Conferir o valor total da compra.
10. Verificar o método de pagamento e as informações de entrega.

### Resultado esperado
O sistema deve permitir o avanço para a página de resumo do pedido e apresentar corretamente as informações da compra, incluindo quantidade, preço do produto, taxa, valor total, método de pagamento e forma de entrega.  

### Resultado obtido
Após preencher todos os campos obrigatórios, o sistema direcionou o usuário para a página de resumo do pedido.
Foi apresentada a quantidade correta de 1 unidade e o preço de $29.99. Também foi apresentada uma taxa de $2.40, resultando no total de $32.39.
O método de pagamento apresentado foi SauceCard e a entrega foi informado como "Free Pny Express Delivery".

### Status
**PASSOU**
