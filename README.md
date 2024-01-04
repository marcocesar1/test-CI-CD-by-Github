# CI/CD Test Project with GitHub Actions

This project is an example of Continuous Integration and Continuous Delivery (CI/CD) using GitHub Actions to automatically deploy to a server via SSH.

## Project Content

The test page (`index.html`) includes a simple message and a test image of ReactJS.

## CI/CD Configuration

### GitHub Actions Workflow

The GitHub Actions workflow is located in the `.github/workflows/main.yml` file. This workflow is triggered on each push to the main branch and performs the following actions:

1. Deploys the files to the server via SSH.

### Deployment

Deployment is done using an SSH private key stored in the repository secrets. The GitHub Actions workflow uses this private key to connect to the server and copy the updated files.

## Accessing the Deployed Project

You can access the deployed project [here](https://phoenix-app.site/ci-cd/).

## Additional Configuration

If you want to replicate this process in your own project, make sure to set up the following secrets in your GitHub repository settings:

- `SSH_PRIVATE_KEY`: The SSH private key used to access the server.
- Other secrets required for your application.

Remember to adjust environment variables and configurations according to your project's specific needs.

Thank you for checking out this CI/CD example with GitHub Actions!
