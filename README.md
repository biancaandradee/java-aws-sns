# AMAZON SNS (Simple Notification Service)
- É um serviço de mensagens totalmente gerenciado para a comunicação de aplicação para aplicação (A2A) e de aplicação para pessoa (A2P).
- A funcionalidade pub/sub de A2A fornece tópicos para sistemas de mensagens de alta taxa de transferência baseados em push e de muitos para muitos entre sistemas distribuídos, microsserviços e aplicações sem servidor orientadas por eventos. Usando tópicos do Amazon SNS, seus sistemas editores podem repassar mensagens para um grande número de sistemas de assinantes, incluindo filas do Amazon SQS, funções do AWS Lambda e endpoints HTTPS e o Amazon Kinesis Data Firehose para processamento paralelo. A funcionalidade A2P permite enviar mensagens para usuários em grande escala por SMS, push de dispositivos móveis e e-mail.

## Clonando projeto de *torneseumprogramador*
git clone https://github.com/torneseumprogramador/java_aws_sns_sender.git

# Criando projeto
mvn archetype:generate -DgroupId=br.com.sqs_sender -DartifactId=sqs_sender -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

# Doc MVN
https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html

### Gerar com manifest
https://www.sohamkamani.com/java/cli-app-with-maven/

# Exemplo Code Base
https://github.com/awsdocs/aws-doc-sdk-examples/tree/main/javav2

### MVN Options
- mvn validate: validate the project is correct and all necessary information is available
- mvn compile: compile the source code of the project
- mvn test: test the compiled source code using a suitable unit testing framework. These tests should not require the code be - packaged or deployed
- mvn package: take the compiled code and package it in its distributable format, such as a JAR.
- mvn integration-test: process and deploy the package if necessary into an environment where integration tests can be run
- mvn verify: run any checks to verify the package is valid and meets quality criteria
- mvn install: install the package into the local repository, for use as a dependency in other projects locally
- mvn deploy: done in an integration or release environment, copies the final package to the remote repository for sharing with other developers and projects.

## Configurando as variáveis de ambiente
- configurar o .bash_profile ou .bashrc
```shell
code ~/.bash_profile

export AWS_ACCESS_KEY="SUA_ACCESS_KEY"
export AWS_SECRET_KEY="SUA_SECRET_KEY"

source ~/.bash_profile
```

## Rodando o projeto
```shell
./build.sh
./start.sh
```

# SNS send to SQS
https://www.youtube.com/watch?v=3y8YubKdtww
