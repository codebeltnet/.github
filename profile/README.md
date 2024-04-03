Provides a set of tools and libraries to help streamline your development efforts in the context of SDLC- and DevSecOps practices.

This ensures a smooth and consistent way to work with your code.

Areas of focus:

- .NET
  - Savvy I/O
  - SharedKernel
  - Bootstrapper
- CI/CD
  - GitHub Actions
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
