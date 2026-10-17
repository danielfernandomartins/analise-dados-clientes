# 📊 Análise de Cancelamento de Clientes com Python

> Projeto de análise exploratória voltado a **comportamento de clientes, churn, experiência do cliente e tomada de decisão**.

## Problema de negócio

Cancelamento de clientes raramente deve ser analisado apenas como um número. A questão mais útil é identificar **quais padrões aparecem com maior frequência entre clientes que cancelam** e como esses sinais podem apoiar ações de retenção.

## Objetivo

Investigar uma base fictícia de clientes e transformar dados brutos em hipóteses úteis para áreas de:

- relacionamento;
- retenção;
- atendimento;
- experiência do cliente;
- operações;
- negócios.

## Perguntas analisadas

- Qual é a incidência de cancelamento na base?
- O tipo de contrato parece relacionado ao churn?
- Clientes que procuram mais o atendimento cancelam mais?
- Atrasos de pagamento aparecem associados ao cancelamento?
- Quais segmentos deveriam receber investigação adicional?

## Etapas da análise

1. leitura e inspeção da base;
2. verificação de qualidade e consistência;
3. tratamento e organização dos dados;
4. análise de distribuição e cancelamento;
5. comparação de comportamento por variáveis relevantes;
6. visualização dos padrões;
7. tradução dos achados em hipóteses de negócio.

## Principais achados da base estudada

- A amostra apresenta taxa elevada de cancelamento.
- Contratos mensais aparecem associados a maior incidência de churn.
- Clientes com maior volume de contatos com atendimento concentram mais cancelamentos.
- Atrasos prolongados de pagamento também aparecem como variável relevante.

> Estes resultados representam associações observadas nesta base de estudo. Eles não comprovam causalidade e precisam de validação estatística e contexto adicional antes de qualquer decisão real de negócio.

## Hipóteses e ações que poderiam ser investigadas

### Contratos mensais
Avaliar se existe diferença de proposta de valor, preço, onboarding ou fidelização em relação a contratos de maior duração.

### Contatos recorrentes com atendimento
Investigar os motivos de contato, resolução no primeiro atendimento e reincidência de problemas. Uma frequência elevada pode indicar fricção na jornada.

### Atrasos em pagamentos
Separar risco financeiro de insatisfação com o serviço. Nem todo atraso significa propensão a churn pelo mesmo motivo.

## O que este projeto demonstra

- limpeza e organização de dados;
- uso de Python e Pandas;
- análise exploratória;
- visualização de dados;
- identificação de padrões;
- formulação de hipóteses;
- conexão entre dados e decisão de negócio;
- comunicação de limitações da análise.

## Tecnologias

**Python** · **Pandas** · **Plotly Express** · **Jupyter Notebook**

## Arquivos

- `analise_cancelamentos.ipynb` — notebook com a análise exploratória;
- `cancelamentos.csv` — base utilizada no estudo.

## Como executar

1. clone o repositório;
2. abra o notebook no VS Code, Jupyter ou Google Colab;
3. garanta que o CSV esteja disponível no mesmo ambiente;
4. execute as células em sequência.

## Limitações

Este é um projeto de análise exploratória e não um modelo preditivo. A base é de estudo e os resultados não devem ser extrapolados para uma operação real sem validação adicional.

## Próximas evoluções

- segmentação mais detalhada de clientes;
- análise de correlação entre variáveis;
- criação de KPIs de retenção;
- dashboard em Power BI;
- versão SQL da análise;
- modelo simples de classificação de churn apenas após criação de baseline e validação adequada.

## Como explicar em entrevista

> "Meu foco não foi apenas calcular churn, mas transformar os padrões observados em perguntas de negócio. Procurei separar correlação de causalidade e mostrar quais análises adicionais seriam necessárias antes de recomendar uma ação."

## Contexto profissional

Escolhi este problema porque conecta tecnologia e dados a temas que fazem parte da minha trajetória: **clientes, relacionamento, indicadores, experiência do cliente e tomada de decisão**.

## Autor

**Daniel Fernando Martins**
