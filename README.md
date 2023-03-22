# @kinde-oss/kinde-nodejs-generator

@kinde-oss/kinde-nodejs-generator - 
The Kinde Nodejs SDK allows developers to generate NodeJS SDK @kinde-oss/kinde-nodejs-sdk [https://github.com/kinde-oss/kinde-nodejs-sdk](https://github.com/kinde-oss/kinde-nodejs-sdk)

## Require
- Java SDK >=8
- Maven

## How to generate kinde-nodejs-generator.jar
1. Open terminal at `openapi-generator` folder
2. Type command: `mvn package -DskipTests`
3. Go to source `.\kinde-nodejs-generator\openapi-generator\modules\openapi-generator-cli\target`
4. Rename file `openapi-generator-cli.jar` to `kinde-nodejs-generator.jar`. 


## How to use
1. Download file kinde-nodejs-generator.jar in repository.
2. Run the following command using npm:

- `java -jar kinde-nodejs-generator.jar generate -i <OpenAPI_specification_name.yml> -g javascript -o <outputDir>`

- Example:

- `java -jar kinde-nodejs-generator.jar generate -i https://kinde.com/api/kinde-mgmt-api-specs.yaml -g javascript -o ./out/myClient`

If you need help connecting to Kinde, please contact us at [support@kinde.com](mailto:support@kinde.com).
