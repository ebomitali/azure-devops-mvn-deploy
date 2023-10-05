# Introduction 
This project exercises the maven deploy to an azure artifact feed
performed using the user agent identity

# Getting Started
Enter you Azure DevOps account where you would create a project, a repo, a pipeline
From Azure DevOps web interface:
- create a project / reuse a project
- create a feed / reuse a feed
- create a repository from these sources
- adjust references to artifact feed within the pom.xml file, both in repositories section and distributionManagement section
- adjust the reference to artifact feed used by MavenAuthenticate task in file azure-pipeline/mvn-deploy.yml
- create a pipeline from azure-pipeline/mvn-deploy.yml file

# Build and Test
Launch the pipeline
Verify successful termination
Enjoy
Currently in a project of mine pipeline execution ends with error and the following message
... status: 403 Forbidden - User '<id of the agent user, something like a68e4335e-...>' lacks permission to complete this action. You need to have 'ReadPackages'...

