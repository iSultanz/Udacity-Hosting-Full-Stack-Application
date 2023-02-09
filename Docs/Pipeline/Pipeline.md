# Pipeline
For sake of continuous integration we used CircleCi to provide and testing for our application and for deployment

## Pipeline process
The pipeline goes through 3 stages to maintain a stability of the application:
1. Build
    - Spin up Environments
    - Preparing environments variables
    - Install Node
    - Install Frontend Dependencies
    - Install API Dependencies
    - Frontend Lint
    - Frontend Build
    - API Build
2. Hold
    - The Pipeline hold and wait for the approval to avoid conflict and problems

3. Deploy
    - Spin up Environments
    - Preparing environments variables
    - Install Node
    - Install AWS CLI - latest
    - Configure AWS Security Credential
    - Deploy App