# 📊 Análise de Desempenho das Lojas - Relatório Final

Este repositório contém uma análise detalhada do desempenho de quatro lojas do Sr. João, o qual me procurar para realizar uma análise estratégica sobre qual dessas 4 lojas ele deveria vender.
A análise levou em conta faturamento de cada loja ao longo de 4 anos, quantidade de vendas de cada loja, categorias mais vendidas, produtos mais e menos vendidos, avaliação dos clientes e desempenho logístico.

[Dashboard para Visualização dos Dados:](https://dashboard-alurastore.streamlit.app/)

[Link do Repositório da Dashboard:](https://github.com/daniel-gramos/dashboard-alurastore)

---

## 🧭 Objetivo

O objetivo desta análise foi comparar o desempenho das lojas em vários aspectos críticos, como:

- **Faturamento Total**
- **Volume de Vendas por Categoria**
- **Avaliação dos Clientes**
- **Desempenho dos Produtos**
- **Custos de Frete e Logística**

Esses dados foram analisados para identificar a loja com o pior desempenho geral, e com isso trazer uma solução para o problema do Sr. João.

---

## 📂 Estrutura do Projeto

- `CSVs/`: Contém os arquivos com os dados brutos utilizados na análise.
- `dashboard/`: Código .py de uma Dashboard desenvolvida com o Streamlit para a visualização dos dados.
- `graficos/`: Arquivos dos gráficos gerados durante o projeto de análise dos dados.
- AluraStore_Daniel_Ramos.ipynb é o arquivo do Jupyter Notebook contendo todos os códigos utilizados para análise do projeto.

---

## 📈 Resultados e Visualizações

### Faturamento das Lojas

As quatro lojas apresentaram um desempenho semelhante em quantidade de vendas (em torno de 2.359 por loja), mas se diferenciam pelo faturamento total e ticket médio, sendo a Loja 1 a campeã em faturamento bruto:

![Faturamento Total de Cada Loja](https://github.com/user-attachments/assets/46197969-d5c4-4682-b732-4ea595e1693c)

---

### Vendas por Categoria

- Eletrônicos e Eletrodomésticos são as categorias mais lucrativas em todas as lojas.
- Livros e Brinquedos têm menor valor agregado, mas mantêm boa rotatividade.
- A Loja 1 lidera nas categorias mais valiosas (eletrônicos, eletrodomésticos).
- A Loja 4 tem menor desempenho geral, mesmo nas categorias fortes.

![Vendas Por Categoria - Cada Loja](https://github.com/user-attachments/assets/0fbb2105-e44d-47d4-932c-2f88d17e63db)

![Valor Total de Vendas por Categoria - Lojas Individuais](https://github.com/user-attachments/assets/2d7e99c7-ab78-4aa5-ae4a-3e101c178122)

---

### Avaliação Média dos Clientes

| Loja  | Nota Média |
|-------|-------------|
| Loja 1 | ⭐ 3.98       |
| Loja 2 | ⭐ 4.04       |
| Loja 3 | ⭐ 4.05       |
| Loja 4 | ⭐ 4.00      |

🔍 **Insight:** A Loja 3 é a melhor avaliada pelos clientes. A Loja 1, embora tenha o maior faturamento, é a que possui a pior nota média de avaliação, o que pode indicar problemas de atendimento ou logística.

![Media Avaliacao Clientes](https://github.com/user-attachments/assets/f3c59c6d-f5f1-42c2-892d-5762d9416e52)

---

### Produtos Mais Vendidos
- Eletrônicos, móveis e eletrodomésticos estão entre os mais vendidos em todas as lojas.
- A **Loja 2** mostra maior equilíbrio entre categorias.

![Top 5 Mais Vendidos por Loja](https://github.com/user-attachments/assets/cfce44a1-ad1e-45d9-8b8a-6434c6f85b0e)
  
### Produtos Menos Vendidos
- Instrumentos musicais e livros aparecem frequentemente entre os menos vendidos.
- A Loja 4 possui maior número de categorias com baixo giro, o que afeta seu desempenho geral.

![Top 5 Menos vendidos por Loja](https://github.com/user-attachments/assets/e48f0dea-13da-4c3f-917d-315f4be22b8a)


---

### Frete Médio por Loja

A análise do custo de frete revelou que a Loja 4 teve o custo médio mais baixo, destacando-se pela sua eficiência logística.

Comparativo de Frete entre lojas:

| Loja |	Frete Médio |	Preço Médio |	% Frete sobre Preço |	Total de Fretes |
|--------|--------|--------|-------|-----------|
|	Loja 1 |	34.69 |	650.49 |	5.33 |	81837.97 |
|	Loja 2 |	33.62 |	630.97 |	5.33 |	79314.16 |
|	Loja 3 |	33.07 |	620.61 |	5.33 |	78022.66 |
|	Loja 4 |	31.28 |	587.15 |	5.33 |	73755.88 |

![Comparativo Frete Dispersão](https://github.com/user-attachments/assets/bb3390de-7e6c-46f6-a860-a7724789f7a0)

Comparativo de Frete por Categoria entre lojas:

| Categoria do Produto |	Qtd de Vendas |	Frete_Medio	| Preco_Medio_Produto |	Frete_Total |	% Frete sobre Preço |
|------------|-----|-----|-------|-----|-----------|
|	Brinquedos |	1290 |	4.16 |	76.08 |	5361.50 |	5.46 |
|	Eletrodomésticos |	1149 |	81.69	| 1537.28 |	93861.63 |	5.31 |
|	Eletrônicos |	1772 |	66.56 |	1249.49 |	117948.36 |	5.33 |
|	Esporte e lazer |	1113 |	9.22 |	171.28 |	10256.55 |	5.38 |
|	Instrumentos musicais |	753 |	32.76 |	617.57 |	24671.81 |	5.31 |
|	Livros |	742 |	3.70 |	67.74 |	2746.69 |	5.46 |
|	Móveis |	1886 |	28.60 |	535.64 |	53935.77 |	5.34 |
|	Utilidades domésticas |	730 |	5.68 |	105.17 |	4148.34 |	5.40 |

![Frete Medio Por Categoria e Loja](https://github.com/user-attachments/assets/8082e900-3353-4821-b6b6-fce5a1b2434d)


---

## 🧾 Recomendação Final

Após analisar todos os aspectos – faturamento, avaliação dos clientes, desempenho por categoria e frete – as lojas se classificam da seguinte forma:

**Ranking Geral de Desempenho:**

1. 🥇 **Loja 1** – Maior faturamento e ticket médio, apesar da menor avaliação.
2. 🥈 **Loja 2** – Boa avaliação e equilíbrio entre categorias.
3. 🥉 **Loja 3** – Média em todos os quesitos.
4. ❌ **Loja 4** – Menor faturamento, menor ticket médio, segunda pior nas avaliações.

👉 **Recomendação final:** O Sr. João deve considerar a **venda da Loja 4**, por apresentar desempenho inferior de forma consistente. Com a venda, ele pode recuperar capital para investir em novas oportunidades ou fortalecer as operações das lojas mais rentáveis.

---

## 🛠️ Tecnologias Utilizadas durante o Projeto

A análise foi realizada utilizando as seguintes ferramentas e bibliotecas:

- **Python**: Linguagem principal para manipulação dos dados.
- **Pandas**: Bibliotecas para tratamento e análise dos dados.
- **Matplotlib**: Ferramenta para visualização gráfica.
- **Seaborn**: Para visualizações estatísticas avançadas.
- **Folium**: Para geração do mapa de calor das vendas.
- **Streamlit**: Geração de uma dashboard interativa para visualização dos dados.

---

📌 **Este projeto foi desenvolvido com fins educativos e demonstra a aplicação de técnicas de análise exploratória de dados.**
