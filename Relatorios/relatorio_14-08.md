# Relatório de Estudos

**Nome do Estagiário:** Giovani Rodrigues 
**Data:** 14/08/24

**Módulos/Etapas Feitas:**  
1. **Linguagens e Frameworks**
2. **Analítico**


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
**Desafios Encontrados:**  

**Feedback e Ajustes:**  
Sem sugestões.

**Próximos Passos:**  
Continuarei me aprofundando e estudando Spark e suas ferramentas.
