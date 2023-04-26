# @kinde-oss/kinde-nodejs-generator

@kinde-oss/kinde-nodejs-generator - 
The Kinde Nodejs SDK allows developers to generate NodeJS SDK @kinde-oss/kinde-nodejs-sdk [https://github.com/kinde-oss/kinde-nodejs-sdk](https://github.com/kinde-oss/kinde-nodejs-sdk)

## Require
- node >= 18.x.x

## Install OpenApi generator
- npm i -g openapi-generator-cli

## Clone the repository to your computer
- git clone https://github.com/kinde-oss/kinde-nodejs-generator

## Change the current working directory
- cd kinde-nodejs-generator

## To generate SDK please run
- openapi-generator-cli generate -g javascript -i <OpenAPI_specification_name.yml> -c config.yaml -o <outputDir> --skip-validate-spec

Example: 
- openapi-generator-cli generate -g javascript  -i https://kinde.com/api/kinde-mgmt-api-specs.yaml -c config.yaml -o ../kinde-nodejs-sdk/ --skip-validate-spec

Folder `kinde-nodejs-sdk` in the parent directory contains our final SDK after build.

If you need help connecting to Kinde, please contact us at [support@kinde.com](mailto:support@kinde.com).
