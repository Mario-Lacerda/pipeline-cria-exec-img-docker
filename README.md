# Desafio Dio - Pipeline de Criação e Execução de uma Imagem Docker



### **Criando um projeto Docker completo**

**Etapa 1: Criar um diretório para o projeto**

- Crie um novo diretório para o seu projeto Docker.

  

**Etapa 2: Criar um arquivo Dockerfile**

- Dentro do diretório do projeto, crie um arquivo chamado `Dockerfile`. Este arquivo conterá as instruções para construir sua imagem Docker.

  

**Etapa 3: Escreva o Dockerfile**

- O Dockerfile deve conter as seguintes instruções:

  

```plaintext
FROM <imagem base>
RUN <comandos para instalar dependências>
COPY <arquivos de código-fonte> <caminho de destino>
RUN <comandos para executar o aplicativo>
```



**Etapa 4: Construir a imagem Docker**

- Execute o seguinte comando para construir a imagem Docker:

```plaintext
docker build -t <nome da imagem> .
```



**Etapa 5: Executar o contêiner Docker**

- Execute o seguinte comando para executar o contêiner Docker:



```plaintext
docker run -it --rm <nome da imagem>
```



**Exemplo de Dockerfile**

Aqui está um exemplo de Dockerfile para um aplicativo Node.js:

```plaintext
FROM node:16-alpine

WORKDIR /usr/src/app

COPY package.json .
RUN npm install

COPY . .

CMD ["node", "index.js"]
```



**Executando o aplicativo**

Depois de construir a imagem Docker, você pode executar o aplicativo executando o contêiner Docker.

1. Execute o seguinte comando para iniciar o contêiner Docker:

```plaintext
docker run -it --rm <nome da imagem>
```

1. O contêiner será iniciado e o aplicativo será executado. Você verá a saída do aplicativo no terminal.





**Conclusão**

Este guia fornece uma visão geral passo a passo sobre como criar e executar uma imagem Docker completa. Seguindo essas etapas, você pode criar e implantar facilmente seus aplicativos em contêineres Docker.













## 230_PipelineCriacaoExecucaoImagemDocker

Pipeline de Criação e Execução de uma Imagem Docker

- CONTEÚDOS
- INFORMAÇÕES



###### DESCRIÇÃO

Neste projeto você deverá criar um pipeline de criação e execução de uma imagem que deverá ser criada e executada em um servidor na nuvem utilizando um Gitlab Runner.



**GitLab**

------

###### Full-Stack

###### Intermediário

------

###### ESPECIALISTA

![author](https://hermes.digitalinnovation.one/users/author/photos/06d27a77-5a11-48fb-9c16-e0c692091bd9.png)

###### Denilson Bonatti

Instrutor, DIO[**](https://www.linkedin.com/in/denilson-bonatti-54a14529/) [**](https://github.com/denilsonbonatti)



https://web.dio.me/project/pipeline-de-criacao-e-execucao-de-uma-imagem-docker/learning/24f8f86e-f134-4560-bcc3-7574fd495821?back=/track/formacao-gitlab-cicd&tab=path&moduleId=f70e9ddf-8de2-489a-945d-3c557e490ff3



Agradecimento ao Ir.´. especial:  

VagnerBellacosa/
