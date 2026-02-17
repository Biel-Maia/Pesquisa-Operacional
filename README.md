# Pesquisa-Operacional


🏋️ Otimização do Planejamento de Treino Baseada no Custo Cardíaco

Este projeto aplica conceitos de Pesquisa Operacional para otimizar a montagem de uma divisão semanal de treinos, considerando o custo cardíaco dos exercícios e a distribuição equilibrada entre grupos musculares.

O problema é modelado como um problema de otimização inteira (MILP) e resolvido utilizando o solver Gurobi, com suporte de bibliotecas como pandas, matplotlib e numpy para manipulação e visualização dos dados.

🎯 Objetivo

Construir automaticamente uma divisão de treinos que:

Minimize o custo cardíaco total

Respeite restrições de frequência por grupo muscular

Mantenha equilíbrio na distribuição dos estímulos

Considere múltiplos grupos musculares por exercício

Produza uma solução viável e eficiente do ponto de vista fisiológico

📊 Etapas do Projeto
1️⃣ Leitura e Processamento de Dados

Importação de planilhas públicas (Google Sheets)

Tratamento e filtragem dos dados

Mapeamento dos exercícios para seus respectivos grupos musculares

Cálculo da frequência de exercícios por grupo

2️⃣ Análise Exploratória

Visualização da distribuição dos exercícios por grupo muscular

Identificação de possíveis desbalanceamentos na base de dados

3️⃣ Modelagem Matemática

O problema é formulado como um modelo de Programação Linear Inteira Mista:

Variáveis de decisão:

Seleção de exercícios

Função objetivo:

Minimizar o custo cardíaco total do planejamento

Restrições incluem:

Quantidade mínima/máxima de exercícios por grupo muscular

Distribuição adequada entre grupos

Restrições estruturais do planejamento

🧠 Ferramentas Utilizadas

Python

Gurobi (solver de otimização)

Pandas

NumPy

Matplotlib

OpenPyXL

📈 Resultados

O modelo gera automaticamente uma seleção otimizada de exercícios que:

Reduz o custo cardíaco acumulado

Mantém equilíbrio muscular

Respeita critérios de divisão definidos

Pode ser adaptado para diferentes cenários (mais grupos, diferentes restrições, etc.)

🚀 Possíveis Extensões

Inserção de restrições relacionadas ao Sistema Nervoso Central (SNC)

Modelagem multiobjetivo (ex: custo cardíaco + volume total)

Personalização por nível (iniciante, intermediário, avançado)

Interface para geração automática de planilhas

Integração com banco de dados

👥 Autores

Gabriel Henrique Silva Maia

Igor Braga de Lima

Talvani de Souza Barbosa

Matheus Gregor Dias Carvalho Costa
