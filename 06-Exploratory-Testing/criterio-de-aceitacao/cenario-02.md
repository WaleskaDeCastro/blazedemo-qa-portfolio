Cenário: Impedir envio com dados inválidos

Dado que o usuário está no formulário de compra
Quando ele inserir dados inválidos
E tentar finalizar a compra
Então o sistema deve impedir o envio
E exibir mensagens de erro nos campos