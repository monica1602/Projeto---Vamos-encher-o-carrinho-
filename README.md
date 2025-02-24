# Projeto de Análise de Dados Vamos encher o carrinho!

## Descrição do Projeto
A Instacart é uma plataforma de entrega de supermercados que permite aos clientes realizarem pedidos online e receberem suas compras em casa, funcionando de maneira semelhante a serviços como Uber Eats e iFood.
O conjunto de dados fornecido foi modificado a partir do original para otimizar a execução dos cálculos. Para isso, o tamanho dos dados foi reduzido, garantindo maior eficiência no processamento. Além disso, valores ausentes e duplicados foram removidos, sem comprometer a representatividade dos dados. Durante as alterações, foi mantida a distribuição original das variáveis, assegurando que os padrões e características dos dados fossem preservados para análises precisas.

## As Tarefas são:
- Limpeza de dados e relatório de hábitos de compra: Remoção de inconsistências, tratamento de valores ausentes e duplicados, seguida da elaboração de um relatório detalhado sobre os padrões de compra dos clientes, como frequência de pedidos, categorias de produtos mais adquiridos e horários de maior demanda.
- Pré-processamento dos dados: Padronização e transformação dos dados para facilitar análises futuras, incluindo ajuste de tipos de colunas, formatação de datas e categorização de produtos.
- Construção de gráficos: Visualização dos dados por meio de gráficos para identificar tendências nos pedidos, como volume de compras ao longo do tempo, distribuição de categorias de produtos e variação do comportamento dos consumidores em diferentes períodos.

## Dicionário de dados
Há cinco tabelas no conjunto de dados. Abaixo está um dicionário que lista as colunas de cada tabela e descreve os dados contidos nelas:
- instacart_orders.csv: cada linha corresponde a um pedido no aplicativo no Instacart
  - 'order_id': é o número de identificação univóco de cada pedido
  - 'user_id': é o número de identificação univóco de cada cliente
  - 'order_number': é o número de vezes que o cliente fez um pedido
  - 'order_dow': é o dia da semana em que o pedido foi feito
  - 'order_hour_of_day': é a hora do dia em que o pedido foi feito
  - 'days_since_prior_order': é o número de dias desde que o cliente fez seu pedido
- products.csv: cada linha corresponde a um produto exclusivo que os clientes podem comprar
  - 'product_id': é o número de identificação exclusivo de cada produto
  - 'product_name': é o nome do produto
  - 'aisle_id': é o número de identificação exclusivo de cada categoria de corredor do supermercado
  - 'department_id': é o número de identificação exclusivo de cada categoria de departamento do supermercado
- order_products.csv: cada linha corresponde a um item incluído em um pedido
  - 'order_id': é o número de identificação exclusivo de cada pedido
  - 'prodcut_id': é o número de identificação exclusivo de cada produto
  - 'add_to_cart_order': é a ordem sequencial em que cada item foi colcoado no carrinho
  - 'recordeed': 0 se o cliente nunca comprou o produto antes, 1 se já o comprou
- aisles.csv
  - 'aisles_id': é o número de identificação exclusivo de cada categoria de corredor do supermercado
  - 'aisle': é o nome do corredor
- department.csv
  - 'department_id': é o número de identificação exclusivo de cada categoria de departmento do supermercado
  - 'department': é o nome do departamento

## Ferramentas e Bibliotecas utilizadas
- Python: Linguagem principal utilizada para manipulação, análise e visualização de dados.
- Pandas: Biblioteca essencial para manipulação e análise de dados estruturados, permitindo organizar informações em DataFrames e Series.
- Matplotlib: Biblioteca voltada para a criação de gráficos e visualizações, auxiliando na interpretação e apresentação dos dados.
- NumPy: Biblioteca que simplifica o manuseio de vetores e matrizes, acelerando cálculos matemáticos e estatísticos nos dados.

## Imagens

### Gráfico - Pedidos por hora
<img src="https://github.com/user-attachments/assets/400dba41-702c-4102-b5f0-2b49eb57e7a9" alt="Projeto 3 - Tabela" width="800"/>

### Gráfico - Dia da semana que as pessoas fazem compras
<img src="https://github.com/user-attachments/assets/99a925c5-9cd5-42fb-9d9a-7afd743b542e" alt="Projeto 3 - Tabela" width="800"/>

### Gráfico - Tempo entre os pedidos
<img src="https://github.com/user-attachments/assets/5b7c06f6-7d96-48d7-82a0-82c2774f0c15" alt="Projeto 3" width="800"/>

### Gráfico - Distribuição do número de pedidos por cliente
<img src="https://github.com/user-attachments/assets/1375d8a3-88f3-43f6-a43a-f5926f0a7b20" alt="Projeto 3" width="800"/>

### Tabela - 20 produtos mais pedidos
<img src="https://github.com/user-attachments/assets/c0de102d-554c-48ad-9b84-443add45b75a" alt="Projeto 3" width="400"/>

### Gráfico - Quantidade de itens por pedido
<img src="https://github.com/user-attachments/assets/151ede78-1fd3-4553-8bc1-a0fa6758629b" alt="Projeto 3" width="800"/>

### Tabela - 20 principais itens incluídos mais frequentemente em pedidos repetidos
<img src="https://github.com/user-attachments/assets/a4d914b9-3ea8-4fe3-8dbc-cc3203c31e16" alt="Projeto 3" width="400"/>

### Tabela - 20 principais itens que as pessoas colocam no carrinho antes de todos os outros
<img src="https://github.com/user-attachments/assets/9b3f7039-c957-450e-a38d-e6abd088b0d8" alt="Projeto 3" width="400"/>

## Resultados
- Horários de maior volume de vendas: A análise gráfica permitiu identificar os períodos do dia com maior número de pedidos, ajudando a entender os momentos de maior demanda.
- Padrão de compras ao longo da semana: Não há uma variação significativa entre os dias da semana, indicando uma distribuição relativamente uniforme dos pedidos.
- Frequência de pedidos: O intervalo entre os pedidos costuma ser inferior a 30 dias, sugerindo um comportamento de compra recorrente entre os clientes.
- Quantidade de pedidos por cliente: A maioria dos clientes realiza entre 1 e 5 pedidos, demonstrando um padrão de consumo moderado.
- Produto mais pedido: Frutas são os itens mais comprados, embora o tipo específico de fruta possa variar entre os clientes.

## Aprendizados
- Análise de dados: Investigação e interpretação das informações para descobrir padrões, tendências e percepções importantes.
- Qualidade dos dados: Verificação da totalidade, consistência e precisão das informações, assegurando a confiabilidade dos resultados.
- Tratamento dos dados: Modificação de tipos de dados, remoção ou preenchimento de valores ausentes e eliminação de duplicatas para assegurar a estrutura adequada para análise.
- Pré-processamento de dados: Preparação dos dados por meio de limpeza, transformação e organização, tornando-os adequados para modelagem e visualização.
- Construção e análise de gráficos: Geração de visualizações para melhor compreensão dos dados, facilitando a identificação de padrões e a tomada de decisões baseadas em evidências.

## Contexto real
- Aplicativos de pedidos variados: Plataformas de pedidos que oferecem diferentes tipos de itens, como comida, supermercado, roupas, eletrônicos, ou uma combinação desses produtos, e que buscam entender melhor o comportamento dos clientes para otimizar a experiência do usuário.
- Empresas que querem entender o comportamento dos clientes: Organizações que utilizam dados para analisar as preferências e hábitos de compra dos consumidores, ajustando suas estratégias de marketing, oferta de produtos e atendimento.
- Lançamento de novos aplicativos: Empreendedores ou empresas que planejam lançar um novo tipo de aplicativo e desejam compreender melhor seu público-alvo para definir funcionalidades e estratégias mais assertivas.
- Analistas de dados de empresas: Profissionais responsáveis pela análise dos dados de consumo para ajudar as empresas a organizar melhor seus estoques, ajustar a quantidade de funcionários necessários e melhorar a logística e a operação como um todo.

## Como executar o Projeto
- Clone o repositório
- Navegue até o diretório do projeto
- Abra o projeto no seu IDE favorito
- Instale as dependências
- Execute o script principal
  
