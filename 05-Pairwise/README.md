# Pairwise Testing – BlazeDemo "Find Flights"

Este projeto apresenta a geração de combinações de teste para a funcionalidade **"Find Flights"** do site BlazeDemo, utilizando a técnica de **Pairwise Testing**.

O objetivo é garantir cobertura eficiente das combinações entre cidades, voos e companhias aéreas, reduzindo o número total de cenários sem perder qualidade de teste.

---

## 🎯 Fatores de Teste

- **Departure City:** Paris, Philadelphia, Boston, Portland, San Diego, Mexico City, Sao Paolo  
- **Destination City:** Buenos Aires, Rome, London, Berlin, New York, Dublin, Cairo  
- **Flight:** 43, 234, 9696, 12, 4346  
- **Airline:** United Airlines, Aer Lingus, Virgin America, Lufthansa  

---

## 🔎 Regras de Negócio Aplicadas

As seguintes regras foram consideradas na modelagem:

- Flight 43 e 12 → Virgin America  
- Flight 234 → United Airlines  
- Flight 9696 → Aer Lingus  
- Flight 4346 → Lufthansa  

Essas restrições garantem que cada número de voo esteja associado corretamente à sua companhia aérea correspondente.

---

## 💡 Objetivo do Projeto

Este projeto demonstra:

- Aplicação prática de Pairwise Testing   
- Organização de cenários para testes funcionais  
- Raciocínio analítico na redução inteligente de combinações  

Projeto desenvolvido para fins de estudo e portfólio em QA.
