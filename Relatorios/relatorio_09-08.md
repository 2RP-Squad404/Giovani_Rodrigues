# Relatório de Estudos

**Nome do Estagiário:** Giovani Rodrigues 
**Data:** 09/08/24

**Módulos/Etapas Feitas:**  
1. **Linguagens e Frameworks**

## Resumo dos módulos 
### Spark
Durante esses dois dias depois do relatório de quarta-feira, continuei estudando Spark. Executei alguns testes, como persistir um dataframe em uma tabela do datawarehouse do Spark, realizar ações e transformações nos dados do dataframe e as diferenças entre o prompt do spark-sql e do pyspark, pois em ambos consigo consultar dados de uma tabela, porém suas sixtaxe e abordações são diferentes: 
~~~bash
spark.sql("select * from clientes").show()
~~~
Nesse caso, estaria consultando o que há na tabela clientes por meio de comandos pyspark.
Porém, se desejasse explorar a mesma tabela usando o SQL puro, poderiamos usar o prompt spark-sql e rodar o seguinte código:
~~~bash
select * from clientes;
~~~
Além da parte prática, pude também aprender sobre alguns conceitos teórico do Spark. Há alguns pontos que queria destacar:
- Dataset: conjunto de dados generalizados. Ele pode receber dados estruturados, semi e não estruturados. O dataset é mais flexivel quando comparado ao dataframe, visto que seu propósito é ser o resultado de uma coleta de dados.
- Dataframe: Estrutura de dados tabular composta por linhas e colunas. Nele, as colunas têm seus próprios tipos de dados especificado. Ele é mais rígido em comparação com o dataset, além de ser imutável.
- Lazy Evaluation: significa que o processo de transformação ocorre quando há uma ação, ou seja, não realizamos a ação de transformação dos dados ainda. Normalmente usamos essa técnica quando queremos ver como ficará depois de executada a ação.
- Tabelas Gerenciadas: são aquelas que o Spark gerencia dados e metadados, tornando possivel alterações.
- Tabelas Não-Gerenciadas: essas são tabelas que o Spark gerencia apenas os metadados, ou seja, ele não pode apagar ou alterar os dados, mas apenas os metadados delas.
- Views: São 'alias' para uma tabela, facilitando a chamada dela para consultas, por exemplo. Há ainda Views globais, que são visíveis em todas as sessões e as de sessão, que são visíveis apenas na sessão.

Vi ainda que o Spark permite trabalhar com outras fontes de dados, como bancos de dados relacionais e não relacionais, possibilitando alterações diretas e a persistência remota.

**Desafios Encontrados:**  
Tive alguns contra-tempos com a VM do Ubuntu (meu laboratório), porém nada me impediu de usar o Putty para me comunicar com ela e executar os exercicios e testes propostos durante o curso de Formação em Spark.

**Feedback e Ajustes:**  
Sem sugestões.

**Próximos Passos:**  
Continuarei me aprofundando e estudando Spark e suas ferramentas.
