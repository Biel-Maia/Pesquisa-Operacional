# 🧮 Otimização de Planejamento de Treino com Programação Linear Inteira (MILP)



## 📌 Visão Geral

Este projeto aplica técnicas de **Pesquisa Operacional** e **Otimização Matemática** para resolver um problema real de tomada de decisão: selecionar um conjunto ótimo de exercícios que minimize o custo fisiológico (custo cardíaco) e, ao mesmo tempo, mantenha equilíbrio entre grupos musculares.

O problema foi modelado como um **Problema de Programação Linear Inteira Mista (MILP)** e resolvido utilizando o **Gurobi Optimizer** em Python.

Mais do que um projeto aplicado ao contexto de treino físico, este trabalho demonstra a capacidade de estruturar problemas reais como modelos matemáticos formais e solucioná-los com ferramentas industriais de otimização.



## 🎯 Problema de Decisão

No planejamento de treinos existe um conflito natural entre:

- Intensidade (custo cardíaco)
- Cobertura adequada dos grupos musculares
- Volume mínimo e máximo por grupo
- Estrutura e coerência do planejamento semanal

A proposta do projeto é substituir decisões heurísticas por um modelo matemático que:

✔ Minimize o custo cardíaco total  
✔ Garanta frequência mínima e máxima por grupo muscular  
✔ Considere exercícios que atuam em múltiplos grupos  
✔ Mantenha consistência estrutural  



## 🧠 Modelagem Matemática



### Variável de Decisão

Variável binária:

xᵢ = 1, se o exercício i for selecionado  
xᵢ = 0, caso contrário  



### Função Objetivo

Minimizar o custo cardíaco total:

min Σ cᵢ xᵢ

Onde:

- cᵢ = custo cardíaco do exercício i  



### Restrições

- Limite mínimo de exercícios por grupo muscular  
- Limite máximo por grupo muscular  
- Restrição opcional de quantidade total de exercícios  
- Tratamento de exercícios que pertencem a múltiplos grupos  

O modelo foi estruturado de forma escalável, permitindo a inclusão de novas restrições sem necessidade de reestruturação completa.



## 🛠 Tecnologias Utilizadas

- Python  
- Gurobi Optimizer  
- Pandas  
- NumPy  
- Matplotlib  
- OpenPyXL  



## 📊 Pipeline do Projeto

1. Importação e tratamento dos dados  
2. Construção da matriz exercício × grupo muscular  
3. Definição dos parâmetros do modelo  
4. Implementação da formulação MILP  
5. Execução do solver  
6. Extração e análise da solução ótima  



## 🚀 Competências Demonstradas

- Modelagem matemática aplicada  
- Formulação de problemas com variáveis binárias  
- Implementação de Programação Linear Inteira  
- Estruturação de sistemas com múltiplas restrições  
- Pensamento analítico e sistêmico  
- Tradução de problema real em modelo computacional  



## 🔎 Aplicabilidade

Embora aplicado ao contexto de treino físico, o modelo é estruturalmente equivalente a problemas como:

- Alocação de recursos  
- Planejamento de produção  
- Escalonamento de tarefas  
- Seleção de portfólio  
- Distribuição balanceada sob restrições  



## 👨‍💻 Autores

- Gabriel Henrique Silva Maia
- Igor Braga de Lima
- Talvani de Souza Barbosa
- Matheus Gregor Dias Carvalho Costa
