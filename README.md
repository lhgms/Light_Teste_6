<p align="center">
    <a href="https://croct.com">
        <img src="https://cdn.croct.io/brand/logo/repo-icon-green.svg" alt="Croct" height="80"/>
    </a>
    <br />
    <strong>Go Project Title</strong>
    <br />
    A brief description about the project.
</p>
<p align="center">
    <img alt="Language" src="https://img.shields.io/badge/language-Go-blue" />
    <img alt="Build" src="https://img.shields.io/badge/build-passing-green" />
    <img alt="Coverage" src="https://img.shields.io/badge/coverage-100%25-green" />
    <img alt="Maintainability" src="https://img.shields.io/badge/maintainability-100-green" />
    <br />
    <br />
    <a href="https://github.com/croct-tech/repository-template-go/releases">📦 Releases</a>
        ·
        <a href="https://github.com/croct-tech/repository-template-go/issues/new?labels=bug&template=bug-report.md">🐞 Report Bug</a>
        ·
        <a href="https://github.com/croct-tech/repository-template-go/issues/new?labels=enhancement&template=feature-request.md">✨ Request Feature</a>
</p>

# Instructions
Follow the steps below to create a new repository:

1. Customize the repository
   1. Click on the _Use this template_ button at the top of this page
   2. Clone the repository locally 
   3. Update the `README.md` and `package.json` with the new package information
2. Setup Code Climate
   1. Add the project to [Croct's code climate organization](https://codeclimate.com/accounts/5e714648faaa9c00fb000081/dashboard)
   2. Go to **Repo Settings > Test coverage** and copy the "_TEST REPORTER ID_"
   3. Go to **Repo Settings > Badges** and copy the maintainability and coverage badges to the `README.md` 
   4. On the Github repository page, go to **Settings > Secrets** and add a secret with name `CC_TEST_REPORTER_ID` and the ID from the previous step as value.
   
## Installation
Use the builtin `go get` to add the package:

```sh
go get github.com/croct-tech/project-go
```

## Basic usage

```go
package main
import (
    "github.com/croct-tech/project-go/packageName"
)

func main() {
    project.Foo()
}
```

## Contributing
Contributions to the package are always welcome! 

- Report any bugs or issues on the [issue tracker](https://github.com/croct-tech/project-go/issues).
- For major changes, please [open an issue](https://github.com/croct-tech/project-go/issues) first to discuss what you would like to change.
- Please make sure to update tests as appropriate.

## Testing

Before running the test suites, the development dependencies must be installed:

```sh
go mod download
```

Then, to run all tests:

```sh
go test
```

Run the following command to check the code against language builtin SAST:

```sh
go vet
```

To validate the language code style and guidelines install [GolangCI-lint](https://golangci-lint.run/usage/install/#local-installation) and run:

```sh
golangci-lint run
```

## Building

For libraries, there is no need to build the project for publishing.  
Binaries can be built using:

```sh
go build
``` 

## License
Copyright © 2015-2020 Croct Limited, All Rights Reserved.

All information contained herein is, and remains the property of Croct Limited. The intellectual, design and technical concepts contained herein are proprietary to Croct Limited s and may be covered by U.S. and Foreign Patents, patents in process, and are protected by trade secret or copyright law. Dissemination of this information or reproduction of this material is strictly forbidden unless prior written permission is obtained from Croct Limited.