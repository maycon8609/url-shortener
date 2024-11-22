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

### Criar pasta out e arquivo de manifesto:
```
Projeto/
├── src/
│   └── main
|       └── java
|           └── com
|               └── maycon
|                   └── Main.java
├── out/
├── META-INF/
│   └── MANIFEST.MF
```

### Execute o comando para instalar as dependências:
```sh
mvn clean install
```

### Manifest (Opcional, para um JAR Executável) `META-INF/MANIFEST.MF`
```
Manifest-Version: 1.0
Main-Class: com.maycon.Main
```

### Compila o codigo para a pasta `out`
```sh
javac -d out src/main/java/com/maycon/Main.java
```

### Gera o arquivo `.jar`
```sh
jar cfm file-name.jar META-INF/MANIFEST.MF -C out .
```

### Executa o Arquivo `.jar`
```sh
java -jar file-name.jar
```
