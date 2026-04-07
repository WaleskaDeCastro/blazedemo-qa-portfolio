Title: Purchase completed successfully with invalid input data

Steps to reproduce:
1. Acessar o site https://blazedemo.com
2. Selecionar origem e destino
3. Clicar em "Find Flights"
4. Escolher um voo
5. Preencher o formulário com dados inválidos (ex: "!!!@@@", "123")
6. Clicar em "Purchase Flight"

Expected result:
O sistema deve validar os dados e impedir a finalização da compra, exibindo mensagens de erro.

Actual result:
A compra é finalizada com sucesso, exibindo a mensagem "Thank you for your purchase today!" mesmo com dados inválidos.

Severity: Critical
Priority: High

Evidence:
![Compra concluída](https://github.com/WaleskaDeCastro/blazedemo-qa-portfolio/blob/main/06-Exploratory-Testing/evidencias/purchase-sucess.png)