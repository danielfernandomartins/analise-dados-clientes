# Análise exploratória de cancelamento de clientes

**Python · Pandas · Plotly Express · Jupyter Notebook**

Estudo de portfólio sobre padrões associados ao cancelamento. A pergunta é: quais segmentos merecem investigação para apoiar hipóteses de retenção?

[Notebook](analise_cancelamentos.ipynb) · [Abrir no Colab](https://colab.research.google.com/github/danielfernandomartins/analise-dados-clientes/blob/main/analise_cancelamentos.ipynb)

## Resultados registrados

Os valores abaixo foram conferidos nas saídas salvas da versão anterior do notebook. Não são uma nova execução nem resultados de uma empresa.

| População analisada | Clientes | Cancelamentos | Taxa |
|---|---:|---:|---:|
| Base após remoção de nulos | 49.996 | 28.393 | 56,79% |
| Recorte sem contratos mensais | 40.112 | 18.509 | 46,14% |
| Recorte anterior, menos de 5 ligações e até 20 dias de atraso | 26.267 | 4.821 | 18,35% |

A leitura inicial registrava 50.000 linhas; quatro foram excluídas por valores ausentes.

**Interpretação:** filtrar clientes altera a população e o denominador. A diferença entre 56,79% e 18,35% não comprova redução de churn e não representa impacto de uma ação de retenção.

Os 9.884 contratos mensais apresentavam cancelamento na execução histórica. Esse padrão exige investigar origem, construção e representatividade da base antes de extrapolar conclusões.

## Método

1. Ler o CSV e verificar colunas obrigatórias e valores do indicador de cancelamento.
2. Inspecionar nulos e registrar quantas linhas são removidas.
3. Calcular a proporção de cancelamentos na base limpa.
4. Comparar contratos e assinaturas com a base completa preservada.
5. Explorar distribuições e comparar recortes explicitamente identificados.

O notebook mantém a base completa e cria variáveis separadas para os recortes. Contagens em histogramas precisam ser interpretadas junto ao tamanho dos segmentos.

**Indicador:** cancelamentos / clientes da população analisada × 100. A coluna `cancelou` usa 1 para cancelamento e 0 para não cancelamento. A janela temporal e a definição operacional original não estão documentadas.

## Reprodução e dados

**Pendência atual:** `cancelamentos.csv` não está incluído no repositório. A origem e a licença ainda precisam ser documentadas. Não é possível reproduzir integralmente os resultados históricos apenas com os arquivos publicados.

Com acesso autorizado ao CSV original:

1. Clone o repositório e entre na pasta.
2. Instale as dependências: `python -m pip install -r requirements.txt`.
3. Coloque `cancelamentos.csv` na pasta do notebook.
4. Abra com `jupyter notebook` e execute as células em sequência.

No Colab, envie o CSV para a sessão antes de executar. O notebook informa claramente a ausência do arquivo. Usar outra base não reproduz os números acima.

## Limitações

- Análise exploratória; não há modelo preditivo ou inferência causal.
- Resultados históricos não foram recalculados nesta revisão, pois o CSV está ausente.
- Remover nulos pode introduzir viés; é necessário avaliar o mecanismo de ausência.
- Limites de ligações e atraso foram escolhidos na exploração e precisam de validação independente.
- Não há demonstração de economia, aumento de receita ou redução real de cancelamentos.
- Origem e licença da base, definição temporal e reprodução integral permanecem pendentes.

## Próximas entregas

- Documentar e disponibilizar a base quando houver permissão.
- Consolidar taxas por segmento com denominadores e análise de qualidade.
- Elaborar uma versão SQL e um dashboard em Power BI.

## Autor

Daniel Fernando Martins · [LinkedIn](https://www.linkedin.com/in/danielfernandomartins)
