# Relatório de Estudos

**Nome do Estagiário:** Giovani Rodrigues 
**Data:** 07/08/24

**Módulos/Etapas Feitas:**  
1. **BigQuery**
2. **Mensageria**
3. **Virtualização**
4. **Linguagens e Frameworks**

## Resumo dos módulos 

### BigQuery
O **BigQuery** é um serviço datawarehouse da GCP usado para análise de dados em larga escala. Ele é totalmente gerenciável, alocando recursos computacionais de maneira autônoma de acordo com a necessidade de processamento. Sua arquitetura baseada em colunas, permite que consultas em Petabytes sejam realizadas em minutos. Essa ferramenta se integra com o ecossistema Google Cloud, permitindo flexibilidade no processo de ingestão de dados, processamento, análise e apresentação. Em se tratando de finanças, o Big Query não cobra pelos dados de carregamento e exportação, porém os custos de armazenamento são baseado no quanto os dados são alterados e na quantidade armazenada. Além do armazenamento, o serviço também cobra pela consulta dos dados, podendo ser do tipo On-demand, custo baseado na quantidade de dados processados, ou Taxa fixa, onde você reserva recursos dedicados para processar dados.

### Mensageria
A **mensageria** tem o objetivo principal de estabelecer comunicação entre diferentes partes de um sistema, permitindo o tráfego de dados de um serviço para o outro.  O Google Cloud Pub/Sub é um serviço de mensageria da GCP. Nele, um publicador envia dados para um Tópico, que é uma entidade onde as mensagens são  publicadas e o assinante, que é o sistema interessado nas mensagens do tópico no qual está inscrito, recebe-as. Este último pode receber as mensagens por push (logo que publicada a mensagens é enviada ao endpoint do assinante), ou por pull (quando o assinante solicita novas mensagens).

Existem outros tipos de mensageria, como a Fila de Mensagens, que tem por característica o armazenamento dos dados em fila, a fim de garantir que eles serão processados em ordem.

### Virtualização
Virtualização é a tecnologia de emular um sistema operacional dentro de um host que já possui seu próprio sistema. A virtualização nos permite criar um ambiente computacional isolado, sem que o host interfira na máquina virtual hospede e vice versa. O software que intermedia esse processo é chamado de Hypervisor. 
Há ainda duas formas de virtualizar um sistema: 
- Bare Metal - as VMs são executadas direto no hardware, sem precisar de um SO host para gerencia-las.
- Hosted - As Vms são executadas dentro de um sistema operacional host, como o Linux rodando no Windows por meio do VirtualBox, software hypervisor.

Os beneficios de se virtualizar um sistema são: aproveitamento de recursos de hardware, escalabilidade e flexibilidade.

### Linguagens e Frameworks

**Python** é uma das principais linguagens para análise de dados. Ela tem diversas bibliotecas que facilitam  o processo de desenvolvimento, como Pandas, Numpy e Matplotlib, ainda contando com suas estruturas de dados nativas, como Tuple, Dictionary, List e Set. Além disso, sua sintaxe simplifica a leitura e interpretação dos códigos escritos.

**Spark** - Esse framework foi criado numa universidade dos Estados Unidos e hoje é mantido pela Apache Software Foundation. Ele é uma ferramenta para processamento de dados que opera em cluster. Seu diferencial no processamento se dá por processar em memória, que é bem mais rápido que o processamento em disco. 
Além disso, Spark ainda possui suporte para linguagens como Java, Python, R e Scala. 

É importante destacar alguns componentes do Spark:
- Job, tarefa a executar;
- Stage, divisão do Job;
- Tasks, menor unidade de trabalho.


**Desafios Encontrados:**  
A conta da udemy da 2RP acaba ficando indisponivel durante metade do período de estágio por excesso de sessões logadas. Isso tem atrapalhado meu processo de estudo dos cursos de Docker, Spark, Hive entre outros.
Além disso, não consegui implementar o ambiente teste do docker. Porém tenho usado uma Vm do Ubuntu para testar o Spark.

**Feedback e Ajustes:**  
Sem sugestões.

**Próximos Passos:**  
Devo continuar no curso de Spark, mas, quando não conseguir continuar o curso, devo estudar outros conteúdos das trilhas.
