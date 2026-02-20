# Pairwise Testing – SauceDemo Login

Este projeto apresenta a geração de **combinações de teste de login** para o site SauceDemo, utilizando o método **Pairwise Testing**.  

O objetivo é **cobrir combinações críticas de Username, Password, Browser e Device**, aumentando a eficiência dos testes sem precisar testar todas as combinações possíveis.

---

## 🎯 Fatores de teste

- **Username:** standard_user, locked_out_user, problem_user, performance_glitch_user, error_user, visual_user  
- **PasswordType:** correct, incorrect, empty  
- **Browser:** Chrome, Firefox, Edge  
- **Device:** Desktop, Mobile  

---

## 💡 Como interpretar

- Cada linha da tabela representa **um cenário de teste de login**.  
- Usuário `locked_out_user` é um caso especial, testado apenas com senha válida.  
- Outras combinações simulam diferentes fluxos de sucesso e erro, cross-browser e cross-device.  
