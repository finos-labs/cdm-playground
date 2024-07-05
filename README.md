![badge-labs](https://user-images.githubusercontent.com/327285/230928932-7c75f8ed-e57b-41db-9fb7-a292a13a1e58.svg)

# CDM Playground

Welcome to the Common Domain Model Playground for Java and Python repository. This project contains source code with native CDM functionalities use cases. It also serves as training material for introductory CDM implementation courses.

## Installation - same as Development setup
OS X & Linux:

```sh
mvn clean install
```

Windows:

```sh
mvn clean install
```

## Usage example

This project can be used to verify the FINOS CDM dependency resolution and resolve CDM-specific implementation questions by running a set of unit tests with widely used functionalities across industry solutions:

- **Serialization:** Basic de/serialization tests from/to JSON using the `RosettaObjectMapper`.
- **Object validation:** Demonstrates the usage of the native `RosettaTypeValidator` evaluating cardinality and business conditions.
- **Qualification:** Product-based qualification mechanism built in CDM using native `QualifyFunctionFactory`.
- **Event driven transitions:** A set of post trade event executions using built-in model functions.

All samples included in the project are publicly available at [FINOS CDM](https://github.com/finos/common-domain-model) repository. The playground project uses samples for the version defined in [pom's](pom.xml) property `finos.cdm.version`

_For more examples and usage, please refer to the [FINOS CDM](https://github.com/finos/common-domain-model)._

## Development setup

The project uses:

- JDK 11
- Maven

```sh
mvn clean verify
```

## Roadmap

List the roadmap steps; alternatively link the Confluence Wiki page where the project roadmap is published.

1. Expand test coverage with functionalities around function binding through dependency injection
2. Expand event execution test coverage 
3. Include a sample event classification application built with CDM python distribution
4. ...

## Contributing

1. Fork it (<https://github.com/finos/cdm-playground/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Read our [contribution guidelines](.github/CONTRIBUTING.md) and [Community Code of Conduct](https://www.finos.org/code-of-conduct)
4. Commit your changes (`git commit -am 'Add some fooBar'`)
5. Push to the branch (`git push origin feature/fooBar`)
6. Create a new Pull Request

## License

Copyright 2024 Trade Header

Distributed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).

SPDX-License-Identifier: [Apache-2.0](https://spdx.org/licenses/Apache-2.0)
