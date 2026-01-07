# Codebelt Engineering Ecosystem

## Purpose & Scope

This repository landscape provides tooling, libraries, and workflows designed to streamline development efforts across the SDLC, with a strong emphasis on DevSecOps practices.

The goal is to ensure a smooth, consistent, and repeatable way of working with code—across development, testing, security analysis, packaging, and deployment.

---

## Table of Contents

- [Purpose & Scope](#purpose--scope)
- [Repository Landscape](#repository-landscape)
  - [Application & Library Repositories (.NET)](#application--library-repositories-net)
  - [CI/CD & Automation](#cicd--automation)
  - [Infrastructure & Runtime](#infrastructure--runtime)
- [Engineering Conventions](#engineering-conventions)
  - [Repository Structure](#repository-structure)
  - [Source Layout (Applications & Libraries)](#source-layout-applications--libraries)
  - [Infrastructure as Code](#infrastructure-as-code)
- [Architectural & Design Principles](#architectural--design-principles)
- [References](#references)
- [Credits & Appreciation](#credits--appreciation)

---

## Repository Landscape

### Application & Library Repositories (.NET)

Core libraries, frameworks, and extensions targeting modern .NET development:

- [Cuemon for .NET](https://github.com/gimlichael/Cuemon)
- [Savvy I/O](https://github.com/codebeltnet/savvyio)
- [Shared Kernel API](https://github.com/codebeltnet/shared-kernel)
- [Unitify API](https://github.com/codebeltnet/unitify)
- [Bootstrapper API](https://github.com/codebeltnet/bootstrapper)
- [Extensions for xUnit API](https://github.com/codebeltnet/xunit)
- [Extensions for BenchmarkDotNet API](https://github.com/codebeltnet/benchmarkdotnet)
- [Extensions for YamlDotNet API](https://github.com/codebeltnet/yamldotnet)
- [Extensions for Globalization API](https://github.com/codebeltnet/globalization)
- [Extensions for Asp.Versioning API](https://github.com/codebeltnet/asp-versioning)
- [Extensions for Swashbuckle.AspNetCore API](https://github.com/codebeltnet/swashbuckle-aspnetcore)
- [Extensions for Newtonsoft.Json API](https://github.com/codebeltnet/newtonsoft-json)
- [Extensions for AWS Signature Version 4 API](https://github.com/codebeltnet/aws-signature-v4)

---

### CI/CD & Automation

#### Reusable Workflows

Composable GitHub Actions workflows intended to standardize CI/CD pipelines:

- [jobs-dotnet-restore](https://github.com/codebeltnet/jobs-dotnet-restore)
- [jobs-dotnet-build](https://github.com/codebeltnet/jobs-dotnet-build)
- [jobs-dotnet-test](https://github.com/codebeltnet/jobs-dotnet-test)
- [jobs-dotnet-pack](https://github.com/codebeltnet/jobs-dotnet-pack)
- [jobs-nuget-push](https://github.com/codebeltnet/jobs-nuget-push)
- [jobs-sonarcloud](https://github.com/codebeltnet/jobs-sonarcloud)
- [jobs-codecov](https://github.com/codebeltnet/jobs-codecov)
- [jobs-codeql](https://github.com/codebeltnet/jobs-codeql)

#### GitHub Actions

Low-level, reusable GitHub Actions used by workflows:

- [dotnet-restore](https://github.com/codebeltnet/dotnet-restore)
- [dotnet-build](https://github.com/codebeltnet/dotnet-build)
- [dotnet-test](https://github.com/codebeltnet/dotnet-test)
- [dotnet-pack](https://github.com/codebeltnet/dotnet-pack)
- [nuget-push](https://github.com/codebeltnet/nuget-push)
- [codecov-scan](https://github.com/codebeltnet/codecov-scan)
- [codeql-scan](https://github.com/codebeltnet/codeql-scan)
- [sonarcloud-scan](https://github.com/codebeltnet/sonarcloud-scan)
- [install-dotnet](https://github.com/codebeltnet/install-dotnet)
- [install-nuget](https://github.com/codebeltnet/install-nuget)
- [minver-calculate](https://github.com/codebeltnet/minver-calculate)
- [git-checkout](https://github.com/codebeltnet/git-checkout)
- [shell-globbing](https://github.com/codebeltnet/shell-globbing)

---

### Infrastructure & Runtime

#### Infrastructure as Code

- Terraform

#### Microservices

- Status Monitor

---

## Engineering Conventions

### Repository Structure

Each repository **must** contain the following at its root:

- `README.md`
- `CONTRIBUTING.md`
- `CODE_OF_CONDUCT.md`
- `LICENSE`
- `CHANGELOG.md`

All ignore files (`.gitignore`, `.dockerignore`, etc.) must also be placed at the root.

---

### Source Layout (Applications & Libraries)

- `src/` — all production source code that is shipped, versioned, and consumed by users (libraries and applications),
- `test/` — all unit, integration, and regression tests that verify correctness and behavior of production code,
- `tooling/` — all internal developer tools and infrastructure used to build, run, analyze, or orchestrate the repository (e.g., benchmark runners, generators, CI helpers),
- `tuning/` — all performance benchmarks and microbenchmarks (BenchmarkDotNet projects) used to measure, compare, and tune runtime characteristics; not correctness tests.

Supporting assets should be placed in dedicated root-level folders, such as:

- `.github`
- `.nuget`
- `.codecov`
- `.docfx`

---

### Infrastructure as Code

Repositories containing IaC should define environment-specific folders:

- `origin` — local development
- `development`
- `staging`
- `production`

---

## Architectural & Design Principles

- SOLID
- DRY
- Consistency
- Generality
- Abstraction
- Modularity
- Separation of Concerns
- Measure Twice, Cut Once

---

## References

- [Microsoft Engineering Guidelines](https://github.com/dotnet/aspnetcore/wiki/Engineering-guidelines)
- [Design Patterns](https://refactoring.guru/design-patterns)
- [Options Pattern](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/configuration/options)
- [Separation of Concerns in Software Design](https://nalexn.github.io/separation-of-concerns/)
- [Clean Code in 5 minutes](https://issuu.com/softhouse/docs/cleancode_5minutes_120523)
- [The Boy Scout Rule](https://biratkirat.medium.com/step-8-the-boy-scout-rule-robert-c-martin-uncle-bob-9ac839778385)
- [Manifesto for Software Craftsmanship](https://manifesto.softwarecraftsmanship.org/)

---

## Credits & Appreciation

Building and maintaining a comprehensive sidecar ecosystem for .NET requires significant effort, ongoing refactoring, and high engineering standards.  
This work is made possible in part through the support of our sponsors, to whom we are sincerely grateful.

### JetBrains

The **JetBrains All Products Pack** has been generously provided by JetBrains in support of **Cuemon for .NET**, part of the Codebelt family of projects.

In particular, **ReSharper** plays a central role in the daily development workflow, contributing directly to code quality, safe refactoring, and long-term maintainability.

### GitHub

We would also like to acknowledge GitHub for providing the platform and tooling that make collaboration, issue tracking, CI/CD workflows, and open-source distribution possible.

GitHub’s infrastructure plays an essential role in enabling transparent development, community contributions, and long-term project visibility.

