# @kinde-oss/kinde-nodejs-generator

@kinde-oss/kinde-nodejs-generator - 
The Kinde Nodejs SDK allows developers to generate NodeJS SDK @kinde-oss/kinde-nodejs-sdk [https://github.com/kinde-oss/kinde-nodejs-sdk](https://github.com/kinde-oss/kinde-nodejs-sdk)

## Require
- Java SDK >=8

## How to use
1. Download file kinde-nodejs-generator.jar in repository.
2. Run the following command using npm:

- `java -jar kinde-nodejs-generator.jar generate -i <OpenAPI_specification_name.yml> -g javascript -o <outputDir> --skip-validate-spec`

- Example:

- `java -jar kinde-nodejs-generator.jar generate -i https://kinde.com/api/kinde-mgmt-api-specs.yaml -g javascript -o ./out/myClient --skip-validate-spec
`

If you need help connecting to Kinde, please contact us at [support@kinde.com](mailto:support@kinde.com).
