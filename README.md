# Crypto_Analysis

Objetivo: análise semanal do mercado Bitcoin e produção automática de um relatório (Word) com gráficos e métricas.

Principais indicadores calculados (explicitamente no código):

2-Year SMA (window=730) e 2-Year MA ×5;

DMA (Displaced Moving Average): deslocamento aplicado ao 2-Year SMA e ao 5×2Y;

Mayer Multiple: Close / 200DMA com linhas de referência (top/bottom levels: 2.4×, 0.75×, 0.65×);

Outros indicadores e operações de scoring (zonas undervalued/overvalued) usados para colorir gráficos e produzir o relatório.

Saídas: gráficos (PNG), relatório Word (.docx) com resumo e interpretação, tabelas com sinais.

Utilidade: obter uma visão consolidada e legível (Word + imagens) para apoiar decisões de longo prazo.

Como usar

Colocar o CSV (p.ex. BTC_EUR Kraken Historical Data.csv) na pasta data/.

Abrir o notebook no Jupyter e executar as células por ordem.

O notebook gera plots e um ficheiro Word com o relatório.

Dependências principais

pandas, matplotlib, pandas_ta (se usado), python-docx (para salvar Word), outras libs standard (numpy, datetime).
