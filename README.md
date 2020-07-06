# openapi


## Step 1 create your API contract

### swagger-editor

- Clone https://github.com/swagger-api/swagger-editor

- [swagger-editor](https://editor.swagger.io/)

- Docker

```bash
docker pull swaggerapi/swagger-editor
docker run -d -p 80:8080 swaggerapi/swagger-editor
```

You can provide your own json or yaml definition file on your host

```bash
docker run -d -p 80:8080 -v $(pwd):/tmp -e SWAGGER_FILE=/tmp/swagger.json swaggerapi/swagger-editor
```

You can provide a API document from your local machine — for example, if you have a file at ./bar/swagger.json:

bash```
docker run -d -p 80:8080 -e URL=/foo/swagger.json -v /bar:/usr/share/nginx/html/foo swaggerapi/swagger-editor   
```



## Step 2 generate your code

### swagger-codegen

- Clone https://github.com/swagger-api/swagger-codegen

- Download

```bash
# Download current stable 3.x.x branch (OpenAPI version 3)
wget https://repo1.maven.org/maven2/io/swagger/codegen/v3/swagger-codegen-cli/3.0.20/swagger-codegen-cli-3.0.20.jar -O swagger-codegen-cli.jar

java -jar swagger-codegen-cli.jar help
```

- Brew

`brew install swagger-codegen`

#### Prereq

- Java 8+

- Apache maven 3.3.3 or greater

#### Running

- Maven

`./mvnw clean package`

- Howebrew

`swagger-codegen generate -i http://petstore.swagger.io/v2/swagger.json -l jaxrs-cxf -o /tmp/gen/`

- Docker

`cd /tmp`

```bash
docker run --rm -v ${PWD}:/local swaggerapi/swagger-codegen-cli generate \
    -i http://petstore.swagger.io/v2/swagger.json \
    -l jaxrs-cxf \
    -o /local/out/jaxrx-cxf
```


#### Help

`config-help –l <some-lang>`

`java -jar modules/swagger-codegen-cli/target/swaggercodegen-cli.jar config-help –l jaxrs-cxf`
