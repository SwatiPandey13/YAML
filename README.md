Create a templates directory in your repository root

Save each of these files in that directory with the corresponding names

The main azure-pipelines.yml file should be in your repository root

You'll need to set up the following service connections in Azure DevOps:

Docker registry

SonarQube

Artifactory (for artifact publishing)

XL Deploy

Required variables that should be defined in your Azure DevOps pipeline or variable groups:

SONAR_TOKEN

SONAR_HOST_URL

ORG_ID (for Snyk)

Artifactory.User

Artifactory.Key

XLD_SERVER_URL

XLD_USER

XLD_PASSWORD

This implementation maintains all the functionality from your Jenkins pipeline while following Azure DevOps best practices. The templates make it easy to reuse components across different projects while keeping the pipeline definition clean and maintainable.
