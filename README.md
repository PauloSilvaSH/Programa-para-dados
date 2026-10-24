> **Portfólio:** [Índice geral dos projetos](https://github.com/PauloSilvaSH/Project_finance_pucrs/blob/main/PORTFOLIO.md) · [README de perfil pronto para publicação](https://github.com/PauloSilvaSH/Project_finance_pucrs/blob/main/README_PROFILE.md)

# Programação para Dados — Análise de Jogos da Steam

Projeto de análise exploratória de um catálogo de jogos da Steam. Os notebooks exploram preços, avaliações do Metacritic, datas de lançamento, publicadoras, gêneros/categorias e suporte a sistemas operacionais.

## Dados
Os notebooks referenciam o arquivo `steam_games.csv`. Ele precisa estar presente no diretório de execução; a documentação não presume uma fonte externa ou atualização automática.

## Projeto 1 — `Fase1.ipynb`
O código:
- Lê o CSV com Pandas.
- Calcula e visualiza a proporção de jogos gratuitos e pagos.
- Converte a data de lançamento para datetime e conta lançamentos por ano.
- Calcula o percentual de jogos com suporte a Windows, macOS e Linux.
- Repete parte das análises em uma amostra limitada às primeiras 20 linhas do arquivo.

## Projeto 2 — `projeto_2.ipynb`
O código contém análises adicionais:
- Converte datas de lançamento e notas do Metacritic para tipos adequados e seleciona os dez jogos mais bem avaliados, usando a data como critério de desempate.
- Filtra jogos de RPG a partir de palavras-chave na descrição e analisa atributos relacionados.
- Identifica publicadoras com mais jogos pagos e compara características dos seus títulos.
- Analisa lançamentos de jogos com suporte a Linux entre 2018 e 2022.
- Calcula a proporção de jogos compatíveis com diferentes sistemas operacionais.
- Investiga jogos single-player e subconjuntos descritos como Indie ou Strategy.
- Usa gráficos para comunicar distribuições e comparações.

## Tecnologias identificadas
Python, Pandas, Matplotlib e Seaborn.

## Como reproduzir
1. Instale `pandas`, `matplotlib` e `seaborn`.
2. Coloque `steam_games.csv` no diretório de execução.
3. Abra e execute os notebooks em Jupyter Notebook, JupyterLab ou ambiente compatível.

## Pontos de atenção e melhorias
- Validar o esquema e os tipos do CSV, especialmente preço, nota do Metacritic e data.
- Usar cópias explícitas ao filtrar DataFrames para evitar avisos de atribuição encadeada.
- Documentar a diferença entre análise do conjunto completo e a amostra das primeiras 20 linhas.
- Ao calcular percentuais, explicitar o denominador e excluir dados ausentes quando necessário.
- Tratar descrições nulas ao buscar palavras-chave e documentar limitações da classificação textual.
- Consolidar código repetido em funções reutilizáveis e incluir requisitos de execução.

## Arquivos principais
- [Fase 1](Fase1.ipynb)
- [Projeto 2](projeto_2.ipynb)
- [Template acadêmico da Fase 1](Template%20-%20Fase%201%20-%20Programa%C3%A7%C3%A3o%20para%20Dados%20(1).pdf)
- [Template acadêmico da Fase 2](Template%20-%20Fase%202%20-%20Programa%C3%A7%C3%A3o%20para%20Dados.pdf)

## Limitações
A documentação reflete os trechos de código inspecionados. A execução completa e a origem/licença do dataset devem ser verificadas antes de redistribuir os dados.
