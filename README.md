# Treinamento: CRT020 - Spark 

Repositório com material preparado em Jupyter Notebook baseado no livro _Spark: The Definitive Guide_, publicado pela editora O'Reilly dos autores Bill Chambers e Matei Zaharia.

Este presente material tem por objetivo, abordar os conceitos chave do Spark de forma a preparar profissionais para a certificação da DataBricks CRT020 - Databricks Certified Associate Developer for Apache Spark 2.4.

<https://academy.databricks.com/exam/databricks-certified-associate-developer-for-apache-spark-24>

Os dados utilizados para este material são fornecidos e são originários do repositório existente criando especialmente para o livro. Dentro deste repositório disponibilizamos os arquivos necessários para o treinamento. 

O repositório original pode ser acessado clonando o repositório a seguir:

```web-idl
https://github.com/databricks/Spark-The-Definitive-Guide.git
```



## Começando

Usamos a API do Python para a confecção desse material. O livro disponibiliza exemplos em Scala e Python. Eventualmente, exemplos em SQL são apresentados de forma a ilustrar as conversões possíveis de comandos SQL em funções nativas do Spark. O Material aborda as definições dos conceitos básicos usados pelo Spark como _RDD_  e _DataFrames_, por exemplo, até os módulos _Streaming_, _ML_ e _Graph_. 

### Pré requisitos

Para seguir esse material é necessário ter o Jupyter Notebook instalado em seu computador. Por se tratar de uma aplicação criada para ambiente distribuído, o Spark pode ser rodado em diversas plataformas. Dentre elas, para esses treinamento, recomenda-se:

- Em maquinas virtuais [(VBox, VMWare), (Cloudera CDH, Hortonworks HDP)]

  Cloudera CDH:

  <https://www.cloudera.com/downloads/cdh/6-1-0.html>

  HortonWorks HDP:

  <https://www.cloudera.com/downloads/hdp.html>

  Oracle VBox:

  <https://www.virtualbox.org/>

- Conteiner

  Docker (Windows):

  <https://docs.docker.com/docker-for-windows/install/>

- Nuvem

  AWS:

  <https://aws.amazon.com/pt/>

  Azure:

  <https://azure.microsoft.com/pt-br/>

  Google Cloud Platform:

  <https://cloud.google.com/>

  

### Instalação

Este material pode ser acessado através do Jupyter Notebook dentro de uma VM com a imagem do SandBox da Hortonworks. Para isso, devemos instalar o jupyter dentro da VM com um procedimento específico descrito em um documento chamado: 
"instrucoesInstalacaoJupyterHorton.txt", de autoria de Eduardo Viana.  

Como o objetivo desse material não é a demonstração de instalação dos diferentes ambientes, disponibilizamos um exemplo simples de como instalar o Spark através de uma imagem Docker que é de fácil instalação, essa instalação já contempla o Jupyter notebook com o Kernel do pyspark: 

```shell
# Rodando o Spark com o Docker
docker run -d -p 8888:8888 -v C:/pastaescolhida/mount:/data jupyter/all-spark-notebook

-p corresponde a porta que vai estar aberta no seu localhost pro jupyter. Então se vc entrar localhost:8888 o jupyter vai estar lá se o docker tiver ativo.

-v corresponde ao volume externo que será montado no docker para passar arquivos (por ex, csvs e jsons).  tudo antes do : significa o volume do seu windows local, depois do : corresponde a pasta que será criada no docker pra comunicação.

# não se esqueça de checar via docker ps se a imagem está ativa e que não há duas imagens rodando ao mesmo tempo.
```

## Feito com

* [Jupyter Notebook](https://jupyter.org/instal) - Aplicação de computação interativa que suporta várias linguagens de programação. 
* [Apache Spark](https://spark.apache.org/) - Mecanismo de análise unificada para processamento de dados em larga escala.



## Autores

* **André Carneiro** 
* **Azize A Fernandes Jr.** 
* **Cindy Silva**



## Licença

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Observações

As variáveis que contiverem caminhos para o acesso de arquivos usados nos notebooks deverão ser adapatadas às arvores de diretório de cada usuário.

