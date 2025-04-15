Provide ways to help you streamline development efforts in the context of SDLC- and DevSecOps practices that ensures a smooth and consistent way of working with code.

Repositories of interest:

- .NET
  - [Savvy I/O](https://github.com/codebeltnet/savvyio)
  - [SharedKernel](https://github.com/codebeltnet/shared-kernel)
  - [Unitify](https://github.com/codebeltnet/unitify)
  - [Bootstrapper](https://github.com/codebeltnet/bootstrapper)
  - [Extensions for xUnit API](https://github.com/codebeltnet/xunit)
  - [Extensions for YamlDotNet API](https://github.com/codebeltnet/yamldotnet)
  - [Extensions for Globalization API](https://github.com/codebeltnet/globalization)
  - [Extensions for Asp.Versioning API](https://github.com/codebeltnet/asp-versioning)
  - [Extensions for Swashbuckle.AspNetCore API](https://github.com/codebeltnet/swashbuckle-aspnetcore)
  - [Extensions for Newtonsoft.Json API](https://github.com/codebeltnet/newtonsoft-json)
  - [Extensions for AWS Signature Version 4 API](https://github.com/codebeltnet/aws-signature-v4)
- CI/CD
  - GitHub Actions
    - [codecov-scan](https://github.com/codebeltnet/codecov-scan)
    - [codeql-scan](https://github.com/codebeltnet/codeql-scan)
    - [codeql-scan-finalize](https://github.com/codebeltnet/codeql-scan-finalize)
    - [docker-compose](https://github.com/codebeltnet/docker-compose)
    - [dotnet-build](https://github.com/codebeltnet/dotnet-build)
    - [dotnet-pack](https://github.com/codebeltnet/dotnet-pack)
    - [dotnet-restore](https://github.com/codebeltnet/dotnet-restore)
    - [dotnet-test](https://github.com/codebeltnet/dotnet-test)
    - [dotnet-tool-install-minver](https://github.com/codebeltnet/dotnet-tool-install-minver)
    - [dotnet-tool-install-reportgenerator](https://github.com/codebeltnet/dotnet-tool-install-reportgenerator)
    - [dotnet-tool-install-sonarscanner](https://github.com/codebeltnet/dotnet-tool-install-sonarscanner)
    - [gcp-download-file](https://github.com/codebeltnet/gcp-download-file)
    - [git-checkout](https://github.com/codebeltnet/git-checkout)
    - [install-dotnet](https://github.com/codebeltnet/install-dotnet)
    - [minver-calculate](https://github.com/codebeltnet/minver-calculate)
    - [nuget-push](https://github.com/codebeltnet/nuget-push)
    - [shell-globbing](https://github.com/codebeltnet/shell-globbing)
    - [sonarcloud-scan](https://github.com/codebeltnet/sonarcloud-scan)
    - [sonarcloud-scan-finalize](https://github.com/codebeltnet/sonarcloud-scan-finalize)
  - Reusable Workflows
    - [jobs-sonarcloud](https://github.com/codebeltnet/jobs-sonarcloud)
    - [jobs-codecov](https://github.com/codebeltnet/jobs-codecov)
    - [jobs-codeql](https://github.com/codebeltnet/jobs-codeql)
    - [jobs-nuget](https://github.com/codebeltnet/jobs-nuget)
- Infrastructure as Code
  - Terraform
- Microservices
  - Status Monitor

## Conventions, Idioms and Patterns

### Repository Structure

In the root of the repository, there should be a `README.md` file with a description of the repository as well as complemental docs such as `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `LICENSE`, `CHANGELOG.md` and so forth.

Any ignore files must also be placed in the root of the repository, including but not limited to `.gitignore`, `.dockerignore` and so forth.

#### Applications and Libraries

The repository must have a `src` folder containing all source code, and a `test` folder containing all unit tests.

Anything that complements your code should be placed in separate sub-folders relative to root, e.g. `.github`, `.nuget`, `.codevoc`, `.docfx` and so forth.

#### Infrastructure as Code

The repository should have the following folders representing the different environments:

- `origin`
- `development`
- `staging`
- `production`

Where `origin` is the local development environment from which the application is being written.

### Principles

- SOLID
- DRY
- Consistency
- Generality
- Abstraction
- Modularity
- Separation of Concerns
  - Same concept as two of the most important design principles of SOLID; SRP and ISP
- Measure Twice, Cut Once

## References

- [Microsoft Engineering Guidelines](https://github.com/dotnet/aspnetcore/wiki/Engineering-guidelines)
- [Design Patterns](https://refactoring.guru/design-patterns)
- [Options Pattern](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/configuration/options?view=aspnetcore-8.0)
- [Separation of Concerns in Software Design](https://nalexn.github.io/separation-of-concerns/)
- [Clean Code in 5 minutes](https://issuu.com/softhouse/docs/cleancode_5minutes_120523)
- [The Boy Scout Rule](https://biratkirat.medium.com/step-8-the-boy-scout-rule-robert-c-martin-uncle-bob-9ac839778385)
- [Manifesto for Software Craftsmanship](https://manifesto.softwarecraftsmanship.org/)
