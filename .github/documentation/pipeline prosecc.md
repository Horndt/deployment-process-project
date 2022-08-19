# CircleCI Pipeline Process

## Start Deploy Process

To start the deploy process, push a new commit into the `master`-branch from the GitHub Repo that is linked with CircleCI.

URL: `https://github.com/Horndt/deployment-process-project.git`

## Build Process Steps

### 1. Install & Lint

- install Node on your system
- install the front-end and then the back-end dependencies
- Lint the front-end code

### 3. Build

- runs the build script for the front-end and then the back-end

### Manual Approval

- after the build steps are successfully done, the pipeline process goes on hold and wait for manual approval.

- if the building process failed, the deployment process ends till the building process completed successfully.

## Deployment Process Steps

### 1. Install

- installing Node on system
- installing and setup eb-cli & aws-cli

### 2.Deploy

- Deploy the back-end

  - installing dependencies
  - Build
  - Set environment variables
  - Deploy with eb-cli

- Deploy the front-end
  - installing dependencies
  - Build
  - deploy with aws-cli

## Workflow

1. Build
2. Manual approval after successful completed building process
3. Deploy
