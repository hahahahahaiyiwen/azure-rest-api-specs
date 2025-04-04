# providerhub

> see https://aka.ms/autorest

This is the AutoRest configuration file for providerhub.

## Getting Started

To build the SDKs for My API, simply install AutoRest via `npm` (`npm install -g autorest`) and then run:

> `autorest readme.md`

To see additional help and options, run:

> `autorest --help`

For other options on installation see [Installing AutoRest](https://aka.ms/autorest/install) on the AutoRest github page.

---

## Configuration

### Basic Information

These are the global settings for the providerhub.

```yaml
openapi-type: arm
openapi-subtype: rpaas
tag: package-2020-11-20
```

### Tag: package-2021-09-01-preview

These settings apply only when `--tag=package-2021-09-01-preview` is specified on the command line.

```yaml $(tag) == 'package-2021-09-01-preview'
input-file:
  - Microsoft.ProviderHub/preview/2021-09-01-preview/providerhub.json
directive:
  - suppress: R4009
    from: providerhub.json
    reason: This version doesn't support systemData.
```

### Tag: package-2021-06-01-preview

These settings apply only when `--tag=package-2021-06-01-preview` is specified on the command line.

```yaml $(tag) == 'package-2021-06-01-preview'
input-file:
  - Microsoft.ProviderHub/preview/2021-06-01-preview/providerhub.json
directive:
  - suppress: R4009
    from: providerhub.json
    reason: This version doesn't support systemData.
```

### Tag: package-2021-05-01-preview

These settings apply only when `--tag=package-2021-05-01-preview` is specified on the command line.

```yaml $(tag) == 'package-2021-05-01-preview'
input-file:
  - Microsoft.ProviderHub/preview/2021-05-01-preview/providerhub.json
directive:
  - suppress: R4009
    from: providerhub.json
    reason: This version doesn't support systemData.
```

### Tag: package-2020-11-20

These settings apply only when `--tag=package-2020-11-20` is specified on the command line.

```yaml $(tag) == 'package-2020-11-20'
input-file:
  - Microsoft.ProviderHub/stable/2020-11-20/providerhub.json
directive:
  - suppress: R4009
    from: providerhub.json
    reason: This version doesn't support systemData.
```

---

# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by AutoRest itself.

```yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-python
  - repo: azure-sdk-for-java
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-ruby
    after_scripts:
      - bundle install && rake arm:regen_all_profiles['azure_mgmt_providerhub']
  - repo: azure-sdk-for-net
  - repo: azure-powershell
```

## CSharp

See configuration in [readme.csharp.md](./readme.csharp.md)

## Python

See configuration in [readme.python.md](./readme.python.md)

## Ruby

See configuration in [readme.ruby.md](./readme.ruby.md)

## TypeScript

See configuration in [readme.typescript.md](./readme.typescript.md)

## Go

See configuration in [readme.go.md](./readme.go.md)

## Java

See configuration in [readme.java.md](./readme.java.md)
