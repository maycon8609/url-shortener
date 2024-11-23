# url-shortener

[![java](https://img.shields.io/badge/java-030712?style=for-the-badge&logo=java)](https://www.java.com/pt-BR/)
[![aws-lambda](https://img.shields.io/badge/aws--lambda-030712?style=for-the-badge&logo=awslambda)](https://aws.amazon.com/pt/lambda/)
[![amazon-s3](https://img.shields.io/badge/amazon--s3-030712?style=for-the-badge&logo=amazons3)](https://aws.amazon.com/pt/s3/)
[![amazon api gateway](https://img.shields.io/badge/amazon_api_gateway-030712?style=for-the-badge&logo=amazonapigateway)](https://aws.amazon.com/pt/api-gateway/)
[![amazon cloud watch](https://img.shields.io/badge/amazon_cloud_watch-030712?style=for-the-badge&logo=amazoncloudwatch)](https://aws.amazon.com/pt/cloudwatch/)

___

## Criar projeto java pelo vscode

### Instale as Extensões Necessárias:
1. **Extension Pack for Java** (inclui suporte ao Java, Maven, Spring, etc.).
2. **Debugger for Java** (separado, caso não venha com o pack).

#### Criar um Projeto Java:
1. Pressione Ctrl+Shift+P e escolha Java: Create Java Project.
2. Escolha No Build Tools para um projeto simples ou Maven/Gradle para projetos mais estruturados.
3. Escolha um diretório para o projeto.
4. O VS Code criará a estrutura básica do projeto com pastas como src e um arquivo Main.java.

### Extrutura de pastas:
```
Projeto/
├── .rest-client/
│   └── api.http
├── .vscode/
│   └── lauch.json
│   └── settings.json
├── assets/
├── src/
│   └── main
│       └── java
│           └── com
│               └── maycon
│                   └── createUrlShortener
│                       └── Main.java
├── target/
├── .gitignore
├── pom.xml
├── readme.md
```

### Para fazer o build usando o proprio vscode(o build sera feito na pasta `target`):
#### `MAVEN -> Lifecycle -> package`
![maven](assets/maven.png)

___

### Executa o Arquivo `.jar`
```sh
java -jar target/url-shortener-1.0-SNAPSHOT.jar
```
