# Relatório de Estudos

**Nome do Estagiário:** Giovani Rodrigues 
**Data:** 14/08/24

**Módulos/Etapas Feitas:**  
1. **Linguagens e Frameworks**
2. **Analítico**
3. **Transacional**


## Resumo dos módulos 
### Módulo 1: Linguagens e Frameworks
Nessa semana, conclui o curso de Formação em Spark com PySpark. Nesse período, pude conhecer ferramentas do Spark para: 
- **Machine Learning:** Embora não tenha gastado muito tempo nesse assunto, observei que o Spark fornece recursos para desenvolver um modelo. O PySpark conta com algumas bibliotecas de inteligência artificial como MLlib, além de conseguirmos trabalhar com bibliotecas do Python como Pandas, Koalas e Numpy.  
- **Spark-Streaming:** utilizamos essa ferramenta da API do Spark quando queremos processar dados a medida que são produzidos. Vale destacar alguns pontos importantes quando iremos trabalhar com streaming: 
    - **Modos de saída:** como sairão os dados:
        - **Append:** apenas novas linhas suporta;
        - **Update:** apenas linhas atualizadas;
        - **Complete:** todo a tabela;
    - **Trigger:** define como funcionará o processamento:
        - **Default:** dispara quando o microbatch termina de ser processado; 
        - **Once:** apenas uma única vez; 
        - **Continuous:** continuamente;
        - **Tempo:** define um intervalo de tempo personalizado;
    - **Checkpointdir:** diretório onde o estado de andamento é salvo.    
**Observação:** No spark temos o conceito de micro-batch, que é um bloco de dados produzidos em intervalo de tempo.

- **Formas de otimizar o processamento:** Temos o Particionamento, que, por padrão, particiona os dados de acordo com o número de núcleos. Bucketing é semelhante ao particionamento, porém estabelece um tamanho fixo de partições. É útil quando temos colunas com alta cardinalidade (valores únicos).

- Cluster: Um cluster do spark é formado por um nó master e workers. Usamos para processamento paralelo, de maneira que as tasks de um job são distribuidas entre os nós.

### Módulo 2: Análitico
Sistemas analíticos são projetados para lidar com análise massiva de dados. O propósito deles é gerar insights sobre uma grande quantidade de dados.  Suas principais características são:
- Escalabilidade, visto que lida com alta quantidade de dados;
- Bom desempenho em consultas, já que sua arquitetura é projetada para consultas ágeis e eficientes;
- Integra dados de diversas fontes, suportando estruturados, não estruturados e semi estruturados.

Um bom exemplo de ferramenta analítica é o Apache Spark, que tem excelente desempenho no processamento de dados por conta da sua arquitetura. Spark opera em memória e pode trabalhar em cluster, capacitando o processamento paralelo. Ele ainda permite maior otimização por meio de particionamento de dados e bucketing.

Outra ferramenta analítica é o BigQuery da GCP, que é uma datawarehouse gerenciável com uma arquitetura baseada em colunas, permitindo consultas rápidas.

Alguns pontos de atenção a observar ao se trabalhar com essas ferramentas são:
- O custo pode ser elevado quando não se tem experiencia ou conhecimento sobre a ferramenta.
- Pode haver dificuldades para implementar o serviço de maneira eficaz.
- Algumas ferramentas podem exigir gerenciamento na escalabilidade.

### Módulo 3: Transacional
São sistemas gerenciadores de banco de dados projetados para facilitar o processamento de transações em tempo real. Eles implementam os princípios ACID para garantir alta nível de confiabilidade, consistência e durabilidade. Além disso, esses gerenciadores de banco de dados devem suportar operações CRUD e garantir baixa latência, para que suas operações sejam rápidas e confiáveis.  Exemplos desses sistemas são: MySQL, Microsoft SQL Server e PostgresSQL. 
É importante observar que todos os bancos de dados transacionais são relacionais. A principal diferença entre eles está no propósito, pois os bancos de dados transacionais são otimizados para garantir operações rápidas e confiáveis, além de ter a capacidade de lidar com alto volume de transações. 

Os maiores desafios no que diz respeito a banco de dados transacionais é a complexidade de gerenciamento, alto custo e escalabilidade horizontal limitada.

No PostgresSQL, por exemplo, temos suporte nativo as propriedades ACID por meio de comandos como BEGIN (inicia a transação), COMMIT (confirma),  ROLLBACK (aborta), e SET transaction isolation level (para configurar o nível de isolamento)

**Desafios Encontrados:**  
Nada a comentar
**Feedback e Ajustes:**  
Sem sugestões.

**Próximos Passos:**  
Começarei a Trilha de Back-end