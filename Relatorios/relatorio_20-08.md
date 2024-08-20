# Relatório de Estudos

**Nome do Estagiário:** Giovani Rodrigues 
**Data:** 20/08/24

**Módulos/Etapas Feitas:**  
1. **System Design**
2. **Docker**


## Resumo dos módulos 

### Módulo 1 - System Design
**System Design** é o processo de desenvolver uma arquitetura de sistema computacional que seja resiliente, consistente e escalonável, atendendo as necessidades da organização.

Alguns pontos importantes a destacar num bom design de sistema são:
- **Escalabilidade:** capacidade de escalar conforme a demanda;
- **Manutenção Básica:** facilidade para manter;
- **Eficiência:** serviço atendendo as necessidades; 
- **Confiabilidade:** garantia de que o sistema é confiável;

Alguns componentes presentes na arquitetura são:
- **Balanceador de Carga:** computador responsável por equilibrar o tráfego de rede, impedindo sobrecarga de requisições a servidores do sistema. Útil para garantir desempenho e disponibilidade dos serviços.
- **Caching:** é uma técnica usada para armazenar temporariamente cópias de dados acessados com frequência, com o objetivo de diminuir a latência das requisições.

### Módulo 2 - Docker
Docker é uma tecnologia usada para facilitar o processo de virtualizar a aplicação sem a necessidade de mais hardware ou de uma VM que emule outro computador. O Docker utiliza ambientes chamados de conteiners para executar as aplicações, de maneira que cada conteiner é isolado e contém apenas o necessário. A vantagem dessa ferramenta é de que ela utiliza o kernel do sistema host para rodar os conteiners.

Para criar um conteiner, precisamos de uma imagem. Essa imagem é responsável por dar as funcionalidades da aplicação, como uma imagem de python, ubuntu e nginx. 

Quando precisamos salvas os dados produzidos por um conteiner, usamos volumes, que são formas de persistir dados da aplicação sem depender do conteiner. Há três tipos de volumes:
- Anonymous - volumes anônimos;
- Named - Volumes nomeados;
- Bind mounts - São salvos fora do Docker.

Para estabelecer comunicação entre conteiners, utilizamos Networks. Networks são formas de gerenciar a conexão no Docker. Temos alguns tipos de conexão, cada uma com sua finalidade:
- Bridge: conexão padrão. Usadas para comunicação entre conteiners;
- Host: permite conexão entre contêiner e host;
- Macvlan: conexão a um contêiner por um MAC address;
- None: sem conexão de rede;
- Plugins: extensões de terceiros;

O Docker ainda nos permite usar uma funcionalidade chamada **Docker Compose**. Com ela podemos definir as conexões de nossa aplicação, Volumes, portas e outras configurações em um único arquivo YAML. Além disso, o Compose é usado para rodar múltiplos conteiners.


**Desafios Encontrados:**  
Nada a comentar

**Feedback e Ajustes:**  
Sem sugestões.

**Próximos Passos:**  
Continuar estudando Docker e seguir para Kubernetes e FastAPI.
