# AWS CodeBuild Environment Variables Lab

This repository contains a simple hands-on lab for practicing **AWS CodeBuild environment variables**.

## What is demonstrated

This lab shows how to use:

- environment variables defined in `buildspec.yml`
- environment variables defined in the **CodeBuild project**
- built-in AWS CodeBuild variables such as:
  - `CODEBUILD_BUILD_ID`
  - `CODEBUILD_BUILD_NUMBER`
  - `CODEBUILD_SOURCE_VERSION`

## Repository contents

- `buildspec.yml` — build instructions for AWS CodeBuild
- `README.md` — project description

## Skills demonstrated

- AWS CodeBuild project setup
- GitHub repository integration with CodeBuild
- working with build-time environment variables
- using built-in CodeBuild variables in build logs
- basic CI workflow troubleshooting

## Example variables used

### From buildspec.yml
- `APP_ENV=dev`
- `LOG_LEVEL=debug`

### From CodeBuild project
- `IMAGE_REPO_NAME=my-demo-app`
- `IMAGE_TAG=v1`

## Goal of the lab

The goal of this lab is to understand how AWS CodeBuild passes variables into the build environment and how they can be used during the build process.

## Notes

This is a training project created for practice related to **AWS Certified DevOps Engineer - Professional (DOP-C02)**.
