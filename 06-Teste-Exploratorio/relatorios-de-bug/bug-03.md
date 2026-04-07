Title: Erro 419 ao tentar login com dados válidos 

Steps to reproduce:
1. Acessar página de login
2. Inserir e-mail no formato válido (ex: teste@teste)
3. Inserir qualquer senha
4. Tentar logar

Expected result:
Sistema deve autenticar usuário ou exibir mensagem clara de erro (ex: credenciais inválidas).

Actual result:
Sistema retorna erro "419 Page Expired".

Severity: Medium
Priority: Medium

Evidence:
![Login](../evidencias/login.png)
![Login](../evidencias/login-error.png)