# Go to Azure devops portal after login with credentials. Please do the following steps.
    - Create a project.
    - Start with Pipelines: Automate your build and release processes.
    - Pre-requisties:
      - Deployments :
        - App server: server to host applications.(Tomcat)
        - Hosted server: physical m/c where app/web server are hosted  
    - Download Apache Tomcat server and install it.
    - Copy source code of application in specific folder.
    - Go to path and run mvn clean install (if it is java appln use maven), it will build war file.
    - Start tomcat server it runs on 8080 port
    - continuous integration: process of automating build and tesing of code everytime a team member commits changes to GIT.
    - continuous delivery: process to build , test, configure and deploy from a build to a production env.

# Demo:
    - Azure pipelines
      - Build pipilines: These pipeline jobs clone the code from assigned repo and build the project based on instructions provided in yml. Typically we use build pipelines to publish artifacts of the project.
      - Release pipeline: These pipelines are generally used to deploy the build artifacts into Agent m/c.
      - Create Release: This component helps us to build end to end pipeline (Connecting build and release pipelines) for CI/CD implementation.