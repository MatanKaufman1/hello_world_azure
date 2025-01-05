Hello World Azure Project

This is a simple .NET "Hello World" application configured with Azure DevOps for CI/CD. The project demonstrates how to build, test, and publish a NuGet package while integrating with SonarQube for code analysis and Azure Artifacts for package management.
Table of Contents

    Project Overview
    Pipeline Overview
    Prerequisites
    How to Run the Pipeline
    NuGet Package Details
    Troubleshooting
    Useful Commands
    Contributions
    License
    Acknowledgments

1. Project Overview

This project is designed as a demonstration of CI/CD pipelines using Azure DevOps. Key features include:

    Building and testing a .NET application.
    Packaging the application as a NuGet package.
    Uploading the package to Azure Artifacts.
    Performing static code analysis with SonarQube.

2. Pipeline Overview

The Azure DevOps pipeline (azure-pipelines.yml) supports the following branches:
dev Branch

    SonarQube Analysis: Ensures code quality.
    Build and Package: Compiles and packages the application.
    Publish to Azure Artifacts: Uploads the NuGet package.
    Email Notification: Sends pipeline status updates via email.

main Branch

    Build and Package: Compiles and packages the application.
    Publish to Azure Artifacts: Uploads the NuGet package.
    Email Notification: Sends pipeline status updates via email.

3. Prerequisites
Tools Required

    Azure DevOps: With a configured agent (matanAgent).
    SonarQube: For static code analysis.
    Azure Artifacts: For managing NuGet packages.

Environment Variables

Ensure the following variables are configured in the pipeline:

    GMAIL_USER: Your Gmail username.
    GMAIL_PASSWORD: Your Gmail app password.

NuGet Feed

Update the nuget.config and azure-pipelines.yml files with your Azure Artifacts feed details.
4. How to Run the Pipeline

    Clone the repository:

    git clone https://github.com/yourusername/hello_world_azure.git
    cd hello_world_azure

    Push changes to the dev or main branch to trigger the pipeline.

    Monitor the pipeline status in Azure DevOps.

5. NuGet Package Details

The NuGet package details are:

    Name: feed-matan
    Version: 1.0.{BuildId}-{SourceBranchName}

Packages are uploaded to the Azure Artifacts feed specified in the pipeline.
6. Troubleshooting
Common Issues

    Pipeline Fails on NuGet Restore:
        Ensure the NuGet feed is correctly configured in nuget.config.
    SonarQube Issues:
        Verify the SonarQube server URL and credentials.
    Email Notifications Fail:
        Check the Gmail username, password, and SMTP configuration.

Useful Commands
Run the Application Locally

cd src
dotnet run

Restore Dependencies

dotnet restore


 Acknowledgments
    Azure DevOps
    SonarQube
    NuGet
