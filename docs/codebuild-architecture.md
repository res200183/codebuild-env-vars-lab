# CodeBuild Architecture

This lab demonstrates a simple CI workflow using AWS CodeBuild.

## Architecture

GitHub Repository
        │
        │ (source)
        ▼
AWS CodeBuild Project
        │
        │ executes
        ▼
buildspec.yml
        │
        │ uses
        ▼
Environment Variables

## Environment Variables Sources

CodeBuild supports several sources of environment variables:

### 1. buildspec.yml variables

Defined directly inside the repository.

Example:

APP_ENV=dev  
LOG_LEVEL=debug

### 2. Project environment variables

Defined in the CodeBuild project configuration.

Example:

IMAGE_REPO_NAME=my-demo-app  
IMAGE_TAG=v1

### 3. Built-in CodeBuild variables

Automatically provided by AWS.

Examples:

CODEBUILD_BUILD_ID  
CODEBUILD_BUILD_NUMBER  
CODEBUILD_SOURCE_VERSION  

These variables allow builds to dynamically adapt to the current source version.

## Typical DevOps Use Case

Environment variables are commonly used to:

- define Docker image tags
- control build environments
- pass configuration values
- integrate with deployment pipelines
