# Template: Projeto Power BI

Resumo
- Título: Nome do projeto
- Objetivo: O que o dashboard responde (ex.: analisar vendas por região)
- Status: Draft / Em desenvolvimento / Concluído

Estrutura sugerida
- /data — amostras CSV/Excel (sem dados sensíveis)
- /pbix — arquivo Power BI Desktop (.pbix)
- /screenshots — imagens dos relatórios para visualização no GitHub
- /docs — documentação, descrição do modelo, principais medidas DAX
- README.md — instruções e resumo do projeto

Como usar
1. Baixe o .pbix em /pbix e abra no Power BI Desktop.
2. Para recriar com dados de exemplo, use os CSVs em /data (detalhados em /docs).
3. Medidas importantes (exemplo):
   - Total Sales = SUM(Sales[Amount])
   - YoY Growth = CALCULATE([Total Sales], SAMEPERIODLASTYEAR(Calendar[Date]))
4. Publicar:
   - Publique no Power BI Service e, se apropriado, use "Publish to web" para gerar um link público.
   - Adicione o link público no README do projeto.

Boas práticas
- Nunca inclua dados sensíveis ou privados em commits públicos.
- Documente as etapas de modelagem (tabelas, chaves, tipo de relacionamento).
- Inclua screenshots com legendas para destacar insights.

Licença
- Escolha uma licença (ex.: MIT) e coloque um arquivo LICENSE no repositório.
