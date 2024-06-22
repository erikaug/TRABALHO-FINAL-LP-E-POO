# TRABALHO-FINAL-LP-E-POO

A aplicação "Loja de Roupas Times de Futebol" é uma aplicação desktop desenvolvida em Java utilizando Swing para a interface gráfica. Ela simula uma loja de roupas que vende camisas de times de futebol. Os principais recursos da aplicação incluem:

1 - Tela de Login e Cadastro: Permite que os usuários façam login ou se registrem na aplicação.

2 - Tela Principal (Vitrine de Produtos): Exibe uma lista de produtos (camisas) disponíveis para compra.

3 - Carrinho de Compras: Permite que os usuários adicionem produtos ao carrinho, visualizem e removam itens do carrinho.

4 - Tela de Pagamento: Facilita o processo de finalização da compra, oferecendo diferentes formas de pagamento.

5 - Tela de Pagamento com Cartão: Detalha a entrada de informações do cartão de crédito ou débito.

![image](https://github.com/erikaug/TRABALHO-FINAL-LP-E-POO/assets/71230803/b8437750-934f-4b12-8b3f-8f14ecef1e1c)


+-------------------+
|   LojaDeRoupas    |
+-------------------+
| - carrinho        |
| - telaPrincipal   |
| - usuarios        |
+-------------------+
| + main(String[])  |
+-------------------+
         |
         | contains
         |
         v
+-------------------+            +-------------------+
|  TelaPrincipal    |<-----------|     Carrinho      |
+-------------------+            +-------------------+
| - panel           |            | - itens           |
| - btnAddCarrinho  |            +-------------------+
| - btnCarrinho     |            | + adicionarItem() |
| - listProdutos    |            | + removerItem()   |
| - produtos        |            | + getItens()      |
+-------------------+            | + calcularTotal() |
| + TelaPrincipal() |            | + limparCarrinho()|
+-------------------+            +-------------------+
         |
         | contains
         |
         v
+-------------------+            +-------------------+
|   TelaCarrinho    |<-----------|    ItemVenda      |
+-------------------+            +-------------------+
| - panel           |            | - produto         |
| - listCarrinho    |            | - quantidade      |
| - btnRemover      |            +-------------------+
| - btnPagamento    |            | + getProduto()    |
+-------------------+            | + getQuantidade() |
| + TelaCarrinho()  |            +-------------------+
| + atualizarLista()|
+-------------------+
         |
         | contains
         |
         v
+-------------------+
|   TelaPagamento   |
+-------------------+
| - panel           |
| - lblTotal        |
| - lblFormaPag.    |
| - txtTotal        |
| - cmbFormaPag.    |
| - btnConfirmar    |
+-------------------+
| + TelaPagamento() |
+-------------------+
         |
         | contains
         |
         v
+-------------------+
| TelaPag.Cartao    |
+-------------------+
| - panel           |
| - lblNumCartao    |
| - lblValidade     |
| - lblCVV          |
| - txtNumCartao    |
| - txtValidade     |
| - txtCVV          |
| - btnConfirmar    |
| - formaPag.       |
+-------------------+
| + TelaPag.Cartao()|
+-------------------+
         |
         | contains
         |
         v
+-------------------+
|    TelaLogin      |
+-------------------+
| - panel           |
| - lblUsuario      |
| - lblSenha        |
| - txtUsuario      |
| - txtSenha        |
| - btnEntrar       |
| - btnCadastrar    |
+-------------------+
| + TelaLogin()     |
+-------------------+
         |
         | contains
         |
         v
+-------------------+
|   TelaCadastro    |
+-------------------+
| - panel           |
| - lblNome         |
| - lblUsuario      |
| - lblSenha        |
| - txtNome         |
| - txtUsuario      |
| - txtSenha        |
| - btnCadastrar    |
+-------------------+
| + TelaCadastro()  |
+-------------------+
         |
         | contains
         |
         v
+-------------------+
|     Produto       |
+-------------------+
| - nome            |
| - preco           |
| - cor             |
+-------------------+
| + getNome()       |
| + getPreco()      |
| + getCor()        |
+-------------------+
         |
         | contains
         |
         v
+-------------------+
|     Usuario       |
+-------------------+
| - nome            |
| - usuario         |
| - senha           |
+-------------------+
| + getNome()       |
| + getUsuario()    |
| + getSenha()      |
+-------------------+
