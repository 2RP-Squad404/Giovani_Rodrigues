# Relatório de Estudos

**Nome do Estagiário:** Giovani Rodrigues 
**Data:** 02/08/24

**Módulos/Etapas Feitas:**  
1. **Engenharia de Dados**
2. **Git**
3. **Computação em Nuvem**
4. **CI/CD**
5. **Linux/Shell**

## Resumo dos módulos 
Começando com **Introdução a Engenharia de Dados**, nesse módulo tive um overview sobre a área. Primeiro, pontos essenciais foram abordados, como o que é a engenharia de dados e o que faz, principais atividades e algumas ferramentas. Esse campo é fundamental para diversas empresas, pois é nele que os dados brutos são transformados em inshgts relevantes.

Já em **Git**, relembrei alguns conceitos e conheci novos, como o Git Flow e seus comandos. Esse modelo de branching é usado para grandes projetos com o objetivo de mantê-los organizados e com qualidade durante o desenvolvimento. Separamos o projeto em duas branches principais: _Master/Main_ (produto final) e _Develop_ (código em produção).Ainda usamos usamos três branches para suporte: Hotfix (correção de erro), Release(Homologação) e Feature (funcionalidades). Além disso, quando iniciamos o Git Flow no nosso repositório local, podemos deixar de usá-lo se assim desejarmos.

Em Computação em Nuvem, foram abordadas algumas ferramentas da GCP úteis para engenharia de dados:
- Google Cloud Dataflow
- Google Cloud Dataproc
- Google Cloud Functions
- Google Cloud Composer

**Dataflow** - É uma ferramenta usada para processamento e análise de dados em larga escala. Ela é um serviço gerenciado pela Google, não precisando configurar e escalonar as instâncias responsáveis pelo processamento de dados. Baseada no Apache Beam, esse serviço é flexível a dados em tempo real(streaming) e batch.

**Dataproc** - Essa ferramenta é usada para processamento de grande volume de dados. Ela utiliza frameworks como Apache Hadoop e Apache Spark e outros para ser flexível a necessidade de processamento. Assim como o DataFlow, ela é totalmente gerenciada, aumentando e reduzindo automaticamente a quantidade de VMs que processam os dados de acordo com a demanda. Além disso, o dataproc é integrado com o ecossistema da Google Cloud, facilitando o processo ETL.

**Composer** - Essa ferramenta tem como objetivo gerenciar o fluxo de trabalho de dados. Ela permite criar, agendar e monitorar pipelines de dados. Esse produto Google é baseado no Apache Airflow, usado para orquestrar fluxos de trabalho de dados.

**Functions** - Essa ferramenta é útil quando queremos programar a execução de um código quando algum evento ocorre. É um produto do tipo Serverless, o que nos permite apenas se preocupar com o código que iremos desenvolver e não com a infraestrutura.

No **módulo CI/CD** foram apresentadas as práticas típicas da cultura DevOps usadas para automatizar os processos de Integração e Entrega/Deploy de um software, com rapidez, segurança e qualidade. O Google Cloud Build é uma ferramenta da GCP usada para criar pipeline CI/CD. Ela permite trabalhar com vários repositórios de código, tais como GitHub, GitLab e BitBucket.

No **módulo Linux-Shell**, conheci alguns pontos de utilização do Shell Script: automação de tarefas, produtividade, administração do sistema e outros. Para testar o que aprendi, desenvolvi um simples script que automatiza o processo de enviar uma nova versão de um código para meu repositório pessoal. Segue o exemplo:
```bash
#!/bin/bash

# colect options
echo "git add ___"
read file_added
git add $file_added

if [$? -d 0]; then
	echo "error!"
	exit 1
else
	echo "sucess!"
	echo
	read -p "Please, enter the commit message" msg
	git commit -m "$msg"

fi
read -p "git push origin ____" branch
read -p "Send? (y/n)" send
if [send -eq "y"]
	git push origin $branch
else
	echo "commit has been detained"
```
Obs: ainda preciso fazer correções e mais testes para validar esse script. Esse foi meu ponto de partida em scripting.


**Desafios Encontrados:**  
Acredito que o maior para mim foi começar a aprender do zero sobre engenharia de dados. Essa nunca foi minha área de interesse, porém pude perceber que, ao começar a me debruçar em estudar, talvez poderia trabalhar nela sem ser insatisfeito e conseguir, a medida de minha competência, entregar os resultados esperados.
