## **CARTA DE TESTE EXPLORATÓRIO – BlazeDemo**

**Data:** 20/03/2026  
**Projeto:** BlazeDemo – Simulador de compra de passagens aéreas  
**URL:** [https://blazedemo.com/index.php](https://blazedemo.com/index.php)  
**Testador(a):** QA  
**Ambiente:** Desktop  
**Navegador:** Google Chrome  
**Duração da sessão:** 60 minutos  
**Tipo de teste:** Exploratório funcional

---

### **1\. OBJETIVO DA SESSÃO**

Explorar o fluxo de compra de passagens aéreas no sistema BlazeDemo, avaliando:

* Comportamento do fluxo de busca de voos  
* Consistência do formulário de compra  
* Validação de dados inseridos  
* Feedback do sistema após ações do usuário  
* Experiência do usuário (UX) durante o processo

O foco é identificar falhas funcionais, ausência de validações e inconsistências de usabilidade.

---

### **2\. ESCOPO**

**Incluído:**

* Seleção de origem e destino de voos  
* Busca de voos (Find Flights)  
* Escolha de voo  
* Preenchimento do formulário de compra  
* Finalização da compra (Purchase Flight)  
* Link promocional “destination of the week”

**Fora de escopo:**

* Integração com sistemas reais de pagamento  
* Testes de segurança  
* Testes de performance

---

### **3\. ESTRATÉGIA DE EXPLORAÇÃO**

* Navegar pelo fluxo principal de compra de passagem  
* Inserir dados válidos e inválidos no formulário  
* Testar comportamento com entradas inconsistentes  
* Explorar links e páginas secundárias  
* Observar mensagens e feedback visual

---

### **4\. FLUXOS TESTADOS**

**4.1 Busca de Voos**

* Seleção de cidades ocorre sem restrições  
* Ao clicar em “Find Flights”, voos são listados

**4.2 Seleção de Voo**

* Usuário pode escolher qualquer voo disponível

**4.3 Formulário de Compra**

* Campos parcialmente preenchidos automaticamente  
* Aceitam qualquer tipo de entrada  
* Não há validação de dados

**4.4 Finalização da Compra**

* Sempre retorna sucesso  
* Exibe mensagem: “Thank you for your purchase today\!”  
* Gera código de confirmação independente dos dados

**4.5 Link Promocional**

* Redireciona para página com imagem (Hawaii)

**4.6 Login**

* O sistema possui validação mínima do formato de e-mail: é necessário incluir pelo menos uma letra ou número antes e depois do “@”

* Se o formato estiver incorreto, aparece a mensagem: *“Please enter a value in the format user@domain”*

* Para a senha, qualquer valor é aceito, mas é necessário preencher algum conteúdo

* Ao tentar logar com e-mail e senha no formato correto, o sistema retorna erro “419 Page Expired”, indicando que a funcionalidade de autenticação ainda não está implementada ou há problema de sessão

* **Observações de QA:**

  * O sistema valida apenas o formato do e-mail, não a autenticidade do usuário

  * Sugestão de melhoria: implementar validação real e feedback claro para credenciais inválidas

---

### **5\. DADOS DE TESTE**

* Dados válidos simulados (ex: nome, cartão fictício)  
* Dados inválidos (ex: “abc123”, “\!\!\!@@@”)  
* Campos em branco  
* E-mail e senha aleatórios no login, respeitando o formato mínimo

---

### **6\. RESULTADOS**

#### **✅ Funcionalidades que funcionaram**

* Navegação entre páginas ocorre corretamente  
* Fluxo até o formulário funciona sem erros  
* Finalização sempre retorna resposta

---

#### **❌ Problemas encontrados**

* Ausência de validação no formulário  
* Sistema aceita qualquer dado  
* Compra finalizada com dados inválidos  
* Login realiza validação mínima de e-mail, mas não válida credenciais reais; retorna erro 419 ao tentar autenticar  
* Falta de mensagens de erro claras


---

#### **⚠ Pontos de melhoria**

* Implementar validações de campos (nome, cartão, etc.)  
* Exibir mensagens de erro claras  
* Implementar validação de autenticação real, com feedback para credenciais inválidas  
* Validar dados antes da compra  
* Melhorar realismo do sistema  
* Melhorar realismo do sistema

---

#### **📘 Aprendizados**

* Testes exploratórios identificam falhas rapidamente  
* Validações são essenciais para confiabilidade  
* UX depende de feedback claro  
* Pensamento crítico é essencial em QA

