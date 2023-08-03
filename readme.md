# Introduction to Visual Studio Code

Visual Studio Code is a lightweight, cross-platform code editor that provides a rich set of features for developers. It supports a wide range of programming languages and frameworks, and has a large ecosystem of extensions that can be used to enhance its functionality.

## Spring Boot Extension Pack

The Spring Boot Extension Pack is a collection of extensions that provide support for developing Spring Boot applications in Visual Studio Code. The extensions included in the pack are:

- Spring Boot Tools
- Spring Boot Dashboard
- Spring Initializr Java Support
- Spring Boot Actuator
- Spring Boot Dashboard - JVM Metrics
- Spring Boot Dashboard - Requests

## Inner Loop Demo

The Inner Loop Demo is a demonstration of the end-to-end Spring development experience in Visual Studio Code. It includes the following steps:

### Getting Started

- Spring Initializr integration
- Use Spring Petclinic from Getting Started guide

### Spring Tooling

- Run the application and access it through the code lenses
- Refresh Live Process connection to update IDE with metrics
- Code navigation, project symbols
- Show live Hovers

### Debugging

- Show debugging flow and hot code replace

### Spring Boot Dashboard

- Show beans, mappings, memory views
- Talk about Spring Boot auto-configuration insights

### Testing

- JUnit Test runner to execute tests without leaving the IDE

### Optional

- Talk about Spring validations - best practices while coding

### Summarize the end-to-end Spring development experience

## Outer Loop Demo

The Outer Loop Demo is a demonstration of the end-to-end Spring development experience in Visual Studio Code, including the steps to check, migrate, build, use GitHub Action, and monitor. It includes the following steps:

### Check

- Scan dependencies for CVEs with Redhat dependency analyzer

### Migrate

- Explain openrewrite recipes from Spring Boot language server
- 3 levels down
- Migrate
- (Optional) Show validations for best practices using openrewrite

### Build

- `mvn package`

### GitHub Action (open springone.yml)

- CodeQL
- Introduce Tanzu build service with Java Azure Buildpack for VMware Tanzu https://network.tanzu.vmware.com/products/tanzu-java-azure-buildpack
- Sets up Microsoft OpenJDK 17 and builds the code
- Commit and deploy to Azure Spring Apps
- Rolled-out deployment

### Monitor

- Open Azure Spring Apps view
- Tanzu live view
- Spring dashboard connect live
  - Beans
  - Endpoint mapping
- Debug live with started node
- (Optional) Azure monitor APM

## Appendix

To create an Azure User for the action:

- `az ad sp create-for-rbac --name springone --role contributor --scopes /subscriptions/<your sub>/resourceGroups/springoneent --sdk-auth`