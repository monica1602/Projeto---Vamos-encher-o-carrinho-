# Projeto de Análise de Dados Vamos encher o carrinho!

## Descrição do Projeto
A Instacart é uma plataforma de entrega de supermercado onde os clientes podem fazer um pedido de supermercado e receber a compra em casa, semelhante ao funcionamento do Uber Eats e do IFood. 
O conjunto de dados que fornecemos foi modificado do original. Foi reduzido o tamanho dele para que os cálculos fossem executados mais rapidamente e foram excluídos valores ausentes e duplicados. Também teve se o cuidado de preservar as distribuições dos dados originais depois das alterações.

## As Tarefas são:
- Limpar os dados e preparar um relatório que forneça informações sobre os hábitos de compra dos clientes da Instacart
- Pré-processamento dos dados
- Construção de gráficos com os pedidos

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
- Python: Linguagem utilizada para análise
- Pandas: Biblioteca para manipulação e análise de dados
- Matplotlib: Biblioteca para gerar gráficos
- Numpy: Biblioteca que permite trabalhar com objetos multidimensionais, como matrizes e sequências

## Imagens

### Pedidos por hora
<img src="https://github.com/user-attachments/assets/400dba41-702c-4102-b5f0-2b49eb57e7a9" alt="Projeto 3 - Tabela" width="200"/>

### Dia da semana que as pessoas fazem compras
<img src="https://github.com/user-attachments/assets/99a925c5-9cd5-42fb-9d9a-7afd743b542e" alt="Projeto 3 - Tabela" width="200"/>

### Tempo entre os pedidos
<img src="https://github.com/user-attachments/assets/5b7c06f6-7d96-48d7-82a0-82c2774f0c15" alt="Projeto 3" width="200"/>

### Distribuição do número de pedidos por cliente
<img src="https://github.com/user-attachments/assets/1375d8a3-88f3-43f6-a43a-f5926f0a7b20" alt="Projeto 3" width="200"/>

### 20 produtos mais pedidos
<img src="https://github.com/user-attachments/assets/c0de102d-554c-48ad-9b84-443add45b75a" alt="Projeto 3" width="200"/>

### Quantidade de itens por pedido
<img src="https://github.com/user-attachments/assets/151ede78-1fd3-4553-8bc1-a0fa6758629b" alt="Projeto 3" width="200"/>

### 20 principais itens incluídos mais frequentemente em pedidos repetidos
<img src="https://github.com/user-attachments/assets/a4d914b9-3ea8-4fe3-8dbc-cc3203c31e16" alt="Projeto 3" width="200"/>

### 20 principais itens que as pessoas colocam no carrinho antes de todos os outros
<img src="https://github.com/user-attachments/assets/9b3f7039-c957-450e-a38d-e6abd088b0d8" alt="Projeto 3" width="200"/>

## Resultados
- Foi possível identificar, através de gráficos, os horários com mais vendas
- Que não existe uma grande variação entre os dias semana
- O intervalo entre os pedidos normalmente é menos de 30 dias
- Através de gráficos, é possível identificar que a maioria dos clientes faz de 1 a 5 pedidos
- O item mais pedidos é fruta, podendo variar no tipo da fruta

## Aprendizados
- Análise de dados
- Qualidade dos dados
- Tratar os dados modificando tipos de dados, valores ausentes, valores duplicados
- Pré-processamento de dados
- Contrução e análise de dados

## Contexto real
- Em um aplicativo real de pedidos, podendo ser apenas de comida, supermercado, roupas, eletrônicos, qualquer outro tipo de item ou uma combinação entre eles
- Aplicativo que gostaria de entender o comportamento de seus clientes
- Empresas ou pessoas que desejam lançar um novo tipo de aplicativo e precisam entender seus possíveis futuros clientes
- Analistas de dados de empresas que desejam entender melhor os clientes para conseguir organizar melhor seus estoques ou quantidade de funcionários

## Como executar o Projeto
- Clone o repositório
- Navegue até o diretório do projeto
- Abra o projeto no seu IDE favorito
- Instale as dependências
- Execute o script principal
  
