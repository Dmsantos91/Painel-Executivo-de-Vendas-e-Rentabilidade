# Painel-Executivo-de-Vendas-e-Rentabilidade
Projeto de Business Intelligence focado em identificar gargalos financeiros, analisar o impacto de descontos na margem de lucro e otimizar a tomada de decisão da diretoria.

📊 Painel Executivo de Vendas e Rentabilidade

<img width="1267" height="812" alt="Painel Executivo de Vendas" src="https://github.com/user-attachments/assets/e556994c-fd3f-48f1-9b48-72c3d75e1de1" />

📌 Visão Geral do Projeto
Em ambientes corporativos complexos, um alto volume de vendas brutas pode frequentemente mascarar margens de lucro espremidas e ineficiências na política de descontos. Este projeto de Business Intelligence (BI) foi desenvolvido para fornecer à diretoria e aos gestores financeiros uma visão clara e acionável sobre a saúde financeira da operação.

O painel transforma dados transacionais brutos em indicadores estratégicos, permitindo o acompanhamento da geração de caixa, ticket médio e a identificação rápida de anomalias na rentabilidade de produtos.

💼 O Problema de Negócio
A operação precisava responder a perguntas vitais para a manutenção do capital de giro e sustentabilidade financeira:

Qual é a margem de lucro real da empresa, além do faturamento bruto?

A atual política de descontos está corroendo a lucratividade de subcategorias específicas?

Quais são os perfis de pagamento (cartão, boleto, etc.) e como eles impactam o fluxo de caixa?

Quais são os 10 principais grupos de produtos (Curva ABC) que sustentam o lucro da organização?

🛠️ Processo de Desenvolvimento (ETL e Modelagem)
1. Extração e Transformação de Dados (Power Query)
Fonte de Dados: Base de dados transacional contendo informações de vendas, clientes, localização e custos.

Limpeza (Data Cleansing): Tratamento de valores ausentes (Nulos/NaN) e ajuste de tipagem de dados para garantir a precisão matemática nas agregações financeiras.

2. Modelagem e Fórmulas Avançadas (DAX)
Para garantir a precisão da análise e permitir a inteligência temporal, a modelagem contemplou:

Tabela dCalendario: Criação de uma dimensão de tempo customizada para viabilizar comparações Mês a Mês (MoM) e Ano a Ano (YoY).

Ticket Médio Real: Utilização da função DISTINCTCOUNT(Order ID) para calcular o ticket médio por pedido emitido, evitando a distorção gerada pela contagem simples de itens comprados no mesmo carrinho.

Segurança Matemática: Uso da função DIVIDE para o cálculo da Margem de Lucro (Total Lucro / Total Vendas), prevenindo erros de divisão por zero.


📈 Visualizações e Insights Estratégicos
O dashboard foi estruturado em uma interface limpa e executiva (UI/UX corporativa), contendo:

KPIs Executivos (Top Level): Faturamento Total, Lucro Líquido, Margem de Lucro Global e Ticket Médio.

Gráfico de Dispersão (Descontos vs. Margem de Lucro): Equipado com uma Linha de Média Analítica, permite a rápida detecção de categorias que perforam abaixo da média aceitável devido a descontos excessivos.

Análise de Curva ABC: Gráfico de barras clusterizado aplicando filtro de Top 10 Subcategorias pelo Lucro (e não por receita), focando no que realmente traz dinheiro para o caixa.

Distribuição de Liquidez: Análise do meio de pagamento para projeção de recebíveis e impacto no capital de giro.

💻 Ferramentas Utilizadas
Microsoft Power BI (Visualização e Relatórios)

Power Query (Processos de ETL)

Linguagem DAX (Expressões de Análise de Dados)

📂 Como visualizar este projeto
(Atenção: Adicione aqui no GitHub uma pasta com imagens/prints em alta qualidade do seu painel finalizado ou suba o arquivo .pbix para download)

Faça o download do arquivo .pbix contido neste repositório.

Abra utilizando o Microsoft Power BI Desktop.

Utilize os filtros de "Ano" e "Região" localizados no cabeçalho para interagir dinamicamente com as métricas financeiras.

Autor: Diego Santos

LinkedIn: https://www.linkedin.com/in/diego-santos-45a72a109/

Focado em transformar dados em previsibilidade financeira e decisões estratégicas.
