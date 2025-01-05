# Hello World Azure Project

This is a simple .NET "Hello World" application configured with Azure DevOps for CI/CD. The project demonstrates how to build, test, and publish a NuGet package while integrating with SonarQube for code analysis and Azure Artifacts for package management.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Pipeline Overview](#pipeline-overview)
3. [Prerequisites](#prerequisites)
4. [How to Run the Pipeline](#how-to-run-the-pipeline)
5. [NuGet Package Details](#nuget-package-details)
6. [Troubleshooting](#troubleshooting)
7. [Useful Commands](#useful-commands)
8. [Contributions](#contributions)
9. [License](#license)
10. [Acknowledgments](#acknowledgments)

---

## Project Overview

This project is designed as a demonstration of CI/CD pipelines using Azure DevOps. Key features include:
- Building and testing a .NET application.
- Packaging the application as a NuGet package.
- Uploading the package to Azure Artifacts.
- Performing static code analysis with SonarQube.

---

## Pipeline Overview

The Azure DevOps pipeline (`azure-pipelines.yml`) supports the following branches:

### dev Branch
- **SonarQube Analysis**: Ensures code quality.
- **Build and Package**: Compiles and packages the application.
- **Publish to Azure Artifacts**: Uploads the NuGet package.
- **Email Notification**: Sends pipeline status updates via email.

### main Branch
- **Build and Package**: Compiles and packages the application.
- **Publish to Azure Artifacts**: Uploads the NuGet package.
- **Email Notification**: Sends pipeline status updates via email.

---

## Prerequisites

### Tools Required
- **Azure DevOps**: With a configured agent (`matanAgent`).
- **SonarQube**: For static code analysis.
- **Azure Artifacts**: For managing NuGet packages.

### Environment Variables
Ensure the following variables are configured in the pipeline:
- **`GMAIL_USER`**: Your Gmail username.
- **`GMAIL_PASSWORD`**: Your Gmail app password.

### NuGet Feed
Update the `nuget.config` and `azure-pipelines.yml` files with your Azure Artifacts feed details.

---

## How to Run the Pipeline

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hello_world_azure.git
   cd hello_world_azure
# Hello World Azure Project

This is a simple .NET "Hello World" application configured with Azure DevOps for CI/CD. The project demonstrates how to build, test, and publish a NuGet package while integrating with SonarQube for code analysis and Azure Artifacts for package management.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Pipeline Overview](#pipeline-overview)
3. [Prerequisites](#prerequisites)
4. [How to Run the Pipeline](#how-to-run-the-pipeline)
5. [NuGet Package Details](#nuget-package-details)
6. [Troubleshooting](#troubleshooting)
7. [Useful Commands](#useful-commands)
8. [Contributions](#contributions)
9. [License](#license)
10. [Acknowledgments](#acknowledgments)

---

## Project Overview

This project is designed as a demonstration of CI/CD pipelines using Azure DevOps. Key features include:
- Building and testing a .NET application.
- Packaging the application as a NuGet package.
- Uploading the package to Azure Artifacts.
- Performing static code analysis with SonarQube.

---

## Pipeline Overview

The Azure DevOps pipeline (`azure-pipelines.yml`) supports the following branches:

### dev Branch
- **SonarQube Analysis**: Ensures code quality.
- **Build and Package**: Compiles and packages the application.
- **Publish to Azure Artifacts**: Uploads the NuGet package.
- **Email Notification**: Sends pipeline status updates via email.

### main Branch
- **Build and Package**: Compiles and packages the application.
- **Publish to Azure Artifacts**: Uploads the NuGet package.
- **Email Notification**: Sends pipeline status updates via email.

---

## Prerequisites

### Tools Required
- **Azure DevOps**: With a configured agent (`matanAgent`).
- **SonarQube**: For static code analysis.
- **Azure Artifacts**: For managing NuGet packages.

### Environment Variables
Ensure the following variables are configured in the pipeline:
- **`GMAIL_USER`**: Your Gmail username.
- **`GMAIL_PASSWORD`**: Your Gmail app password.

### NuGet Feed
Update the `nuget.config` and `azure-pipelines.yml` files with your Azure Artifacts feed details.

---

## How to Run the Pipeline

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hello_world_azure.git
   cd hello_world_azure
# Hello World Azure Project

This is a simple .NET "Hello World" application configured with Azure DevOps for CI/CD. The project demonstrates how to build, test, and publish a NuGet package while integrating with SonarQube for code analysis and Azure Artifacts for package management.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Pipeline Overview](#pipeline-overview)
3. [Prerequisites](#prerequisites)
4. [How to Run the Pipeline](#how-to-run-the-pipeline)
5. [NuGet Package Details](#nuget-package-details)
6. [Troubleshooting](#troubleshooting)
7. [Useful Commands](#useful-commands)
8. [Contributions](#contributions)
9. [License](#license)
10. [Acknowledgments](#acknowledgments)

---

## Project Overview

This project is designed as a demonstration of CI/CD pipelines using Azure DevOps. Key features include:
- Building and testing a .NET application.
- Packaging the application as a NuGet package.
- Uploading the package to Azure Artifacts.
- Performing static code analysis with SonarQube.

---

## Pipeline Overview

The Azure DevOps pipeline (`azure-pipelines.yml`) supports the following branches:

### dev Branch
- **SonarQube Analysis**: Ensures code quality.
- **Build and Package**: Compiles and packages the application.
- **Publish to Azure Artifacts**: Uploads the NuGet package.
- **Email Notification**: Sends pipeline status updates via email.

### main Branch
- **Build and Package**: Compiles and packages the application.
- **Publish to Azure Artifacts**: Uploads the NuGet package.
- **Email Notification**: Sends pipeline status updates via email.

---

## Prerequisites

### Tools Required
- **Azure DevOps**: With a configured agent (`matanAgent`).
- **SonarQube**: For static code analysis.
- **Azure Artifacts**: For managing NuGet packages.

### Environment Variables
Ensure the following variables are configured in the pipeline:
- **`GMAIL_USER`**: Your Gmail username.
- **`GMAIL_PASSWORD`**: Your Gmail app password.

### NuGet Feed
Update the `nuget.config` and `azure-pipelines.yml` files with your Azure Artifacts feed details.

---

## How to Run the Pipeline

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hello_world_azure.git
   cd hello_world_azure
2. Push changes to the dev or main branch to trigger the pipeline.
3. Monitor the pipeline status in Azure DevOps.

---

## Troubleshooting
Common Issues

    Pipeline Fails on NuGet Restore:
        Ensure the NuGet feed is correctly configured in nuget.config.
    SonarQube Issues:
        Verify the SonarQube server URL and credentials.
    Email Notifications Fail:
        Check the Gmail username, password, and SMTP configuration.

---
## Useful Commands
Run the Application Locally

cd src
dotnet run

Restore Dependencies

dotnet restore

---

## Acknowledgments

Special thanks to the following tools and platforms:

    Azure DevOps
    SonarQube
    NuGet2. Push changes to the dev or main branch to trigger the pipeline.
3. Monitor the pipeline status in Azure DevOps.

---

## Troubleshooting
Common Issues

    Pipeline Fails on NuGet Restore:
        Ensure the NuGet feed is correctly configured in nuget.config.
    SonarQube Issues:
        Verify the SonarQube server URL and credentials.
    Email Notifications Fail:
        Check the Gmail username, password, and SMTP configuration.

---
## Useful Commands
Run the Application Locally

cd src
dotnet run

Restore Dependencies

dotnet restore

---

## Acknowledgments

Special thanks to the following tools and platforms:

    Azure DevOps
    SonarQube
    NuGet
