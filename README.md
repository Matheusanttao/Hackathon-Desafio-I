# Hackathon-Desafio-I
# Desafio de Engenharia de Dados com AdventureWorks

Este projeto foi desenvolvido como parte do Desafio de Engenharia de Dados, utilizando o dataset público AdventureWorks. O AdventureWorks é um banco de dados de exemplo que representa uma empresa fictícia de comércio de bicicletas e acessórios, chamada Adventure Works Cycles.

## Estrutura do Projeto

- `database/`: Contém o diagrama ER e scripts SQL para criar e carregar o banco de dados.
- `queries/`: Contém os arquivos SQL com as queries para responder às perguntas de negócio.
- `visualizations/`: Contém os scripts para gerar as visualizações de dados.
- `data/`: Contém os arquivos CSV exportados com os resultados das queries.
- `notebooks/`: Contém os notebooks Jupyter usados para análise e visualização de dados.

## Tarefas Realizadas

### Tarefa I: Carregamento do Dataset

1. **Download e Importação**:
    - O dataset AdventureWorks foi baixado e carregado no banco de dados.
    - Diagrama Entidade-Relacionamento (ER) foi criado para visualizar as relações entre as tabelas.
    - Base SQL foi criada a partir do diagrama ER e arquivos CSV.

### Tarefa II: Queries SQL

As seguintes queries foram elaboradas para responder às perguntas de negócio:

1. **Top 10 Produtos Mais Vendidos na Categoria "Bicicletas" nos Últimos Dois Anos**:
    ```sql
    -- Query para listar os 10 produtos mais vendidos na categoria "Bicicletas" nos últimos dois anos
    ```

2. **Cliente com o Maior Número de Pedidos Realizados no Último Ano Fiscal**:
    ```sql
    -- Query para encontrar o cliente com o maior número de pedidos realizados no último ano fiscal
    ```

3. **Mês com Mais Vendas em Valor Total, Considerando Receita Média Acima de 500 Unidades**:
    ```sql
    -- Query para identificar o mês com mais vendas (em valor total) com receita média por venda acima de 500 unidades
    ```

4. **Vendedores com Vendas Acima da Média no Último Ano Fiscal e Crescimento de Vendas Superior a 10%**:
    ```sql
    -- Query para listar os vendedores com vendas acima da média no último ano fiscal e crescimento de vendas superior a 10%
    ```

5. **Pergunta de Negócio Adicional**:
    ```sql
    -- Query para responder a uma pergunta de negócio adicional utilizando subconsultas, funções de janela ou CTEs
    ```

### Tarefa Extra: Visualizações de Dados

As seguintes visualizações foram criadas para fornecer insights sobre o desempenho da empresa:

1. **Gráfico de Linha - Tendência das Vendas Totais ao Longo do Tempo**:
    - Mostra a tendência das vendas totais mensalmente, destacando meses de pico e adicionando uma linha de tendência para prever vendas futuras.
    - Código: `visualizations/sales_trend.py`

2. **Gráfico de Barras - Top 10 Produtos Mais Vendidos na Categoria "Bicicletas"**:
    - Apresenta a quantidade vendida e o lucro gerado por produto na categoria de "Bicicletas".
    - Código: `visualizations/top_10_bicycles.py`

3. **Mapa de Calor - Vendas por Região e Mês**:
    - Ilustra as vendas por região e por mês, com capacidade de filtrar por categorias de produtos.
    - Código: `visualizations/sales_heatmap.py`

4. **Gráfico de Dispersão - Relação entre Número de Vendas e Valor Total por Cliente**:
    - Mostra a relação entre o número de vendas e o valor total das vendas por cliente, com uma linha de regressão para destacar a tendência.
    - Código: `visualizations/sales_scatter.py`

5. **Gráfico de Barras Empilhadas - Comparação de Vendas Mensais de Dois Anos Consecutivos**:
    - Compara as vendas mensais de dois anos consecutivos, permitindo uma análise detalhada das tendências de crescimento ou declínio por categoria de produto.
    - Código: `visualizations/sales_comparison.py`

## Tecnologias Utilizadas

- **Python**: Para análise e visualização de dados.
- **SQL**: Para consultas no banco de dados.
- **Jupyter Notebooks**: Para desenvolvimento interativo e visualização.
- **Matplotlib/Seaborn/Plotly**: Para criação das visualizações.
- **SQLite/PostgreSQL**: Para armazenar e manipular os dados.

## Passo-a-Passo para Reproduzir o Projeto

1. Clone o repositório:
    ```bash
    git clone https://github.com/SEU_USUARIO/adventureworks-datascience.git
    cd adventureworks-datascience
    ```

2. Configure o ambiente:
    - Crie um ambiente virtual e ative-o:
        ```bash
        python -m venv venv
        source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
        ```
    - Instale as dependências:
        ```bash
        pip install -r requirements.txt
        ```

3. Carregue o banco de dados:
    - Execute os scripts SQL em `database/` para criar e carregar o banco de dados.

4. Execute as queries:
    - As queries SQL estão em `queries/`. Você pode executá-las diretamente no banco de dados.

5. Gere as visualizações:
    - Execute os scripts em `visualizations/` para gerar os gráficos.

## Resultados das Queries

Os resultados das queries SQL foram exportados para arquivos CSV e estão localizados na pasta `data/`.

## Interpretações

Durante a solução do exercício, foram feitas as seguintes premissas e interpretações:

- Apenas vendas dos últimos dois anos foram consideradas para as queries relevantes.
- Clientes que fizeram pelo menos um pedido em cada trimestre do último ano fiscal foram considerados para a análise de clientes.
- As visualizações foram criadas com base nos dados disponíveis no dataset AdventureWorks e refletem os insights sobre o desempenho da empresa.

## Conclusão

Este projeto fornece uma análise abrangente dos dados da AdventureWorks, respondendo a perguntas de negócio específicas e fornecendo insights visuais sobre o desempenho da empresa. Sinta-se à vontade para explorar e expandir este projeto conforme necessário.
