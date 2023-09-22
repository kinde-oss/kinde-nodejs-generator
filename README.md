# Kinde Nodejs generator

The generator for the [Kinde Nodejs SDK](https://github.com/kinde-oss/kinde-nodejs-sdk).

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com) [![Kinde Docs](https://img.shields.io/badge/Kinde-Docs-eee?style=flat-square)](https://kinde.com/docs/developer-tools) [![Kinde Community](https://img.shields.io/badge/Kinde-Community-eee?style=flat-square)](https://thekindecommunity.slack.com)

## Overview

This generator creates an SDK in Nodejs that can authenticate to Kinde using the Authorization Code grant or the Authorization Code with PKCE grant via the [OAuth 2.0 protocol](https://oauth.net/2/). It can also access the [Kinde Management API](https://kinde.com/api/docs/#kinde-management-api) using the client credentials grant.

Also, see the SDKs section in Kinde’s [contributing guidelines](https://github.com/kinde-oss/.github/blob/main/.github/CONTRIBUTING.md).

## Usage

### Initial set up

1. Clone the repository to your machine:

   ```bash
   git clone https://github.com/kinde-oss/kinde-nodejs-generator.git
   ```

2. Go into the project:

   ```bash
   cd kinde-nodejs-generator
   ```

3. Install the OpenAPI Generator tool:

   https://openapi-generator.tech/docs/installation

### SDK generation

Run the following command to generate the SDK:

```bash
openapi-generator-cli generate -g javascript -i <OpenAPI_specification_name.yml> -c config.yaml -o <outputDir> --skip-validate-spec
```

**Note:** The API specifications should always point to Kinde's hosted version: https://kinde.com/api/kinde-mgmt-api-specs.yaml. This is set via the ` -i` option in the [OpenAPI Generator CLI](https://openapi-generator.tech/docs/usage/), for example:

```bash
openapi-generator-cli generate -i https://kinde.com/api/kinde-mgmt-api-specs.yaml
```

The SDK gets outputted to: `kinde-nodejs-sdk`, which you can enter via:

```bash
cd kinde-nodejs-sdk
```

## SDK documentation

[Nodejs SDK](https://kinde.com/docs/developer-tools/nodejs-sdk)

## Contributing

Please refer to Kinde’s [contributing guidelines](https://github.com/kinde-oss/.github/blob/489e2ca9c3307c2b2e098a885e22f2239116394a/CONTRIBUTING.md).

## License

By contributing to Kinde, you agree that your contributions will be licensed under its MIT License.
