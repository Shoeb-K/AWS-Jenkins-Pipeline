# Jenkins AWS CI/CD Pipeline

## Overview

This repository provides a guide on setting up a robust CI/CD pipeline using Jenkins, AWS CodeBuild, and AWS CodeDeploy. The integration allows for automatic deployment of artifacts produced by AWS CodeBuild using AWS CodeDeploy, resulting in a streamlined development workflow.

![Pipeline Overview](https://user-images.githubusercontent.com/48589838/89983289-e5fc2900-dc94-11ea-9258-685375cad1dd.png)

### Walkthrough

1. **Create Resources:** Launch an AWS CloudFormation template to create essential infrastructure components, including S3 buckets, IAM roles, Jenkins server, CodeBuild project, CodeDeploy application, and more.

   ![Resource Creation](https://user-images.githubusercontent.com/48589838/89985330-87d14500-dc98-11ea-9964-c1211d0c8a03.png)

2. **Access and Unlock Jenkins Server:** Retrieve the JenkinsServerDNSName from the CloudFormation stack Outputs tab, access the server, and unlock Jenkins using the provided instructions.

   ![Unlock Jenkins](https://user-images.githubusercontent.com/48589838/89985442-ba7b3d80-dc98-11ea-9cb4-9014339ba6e3.png)

3. **Create Project and Configure CodeDeploy Jenkins Plugin:** Set up a Jenkins project and configure the CodeDeploy Jenkins plugin for seamless integration.

   ![Configure Jenkins](https://user-images.githubusercontent.com/48589838/89985612-fadabb80-dc98-11ea-84cf-c2add128ffc0.png)

4. **Testing the CI/CD Pipeline:** Put an application on your GitHub repository, trigger the pipeline by pushing code changes, and monitor the build and deployment process through Jenkins.

   ![Pipeline Testing](https://user-images.githubusercontent.com/48589838/89986214-d92e0400-dc99-11ea-84cb-9ff3e830a1b8.png)

   View detailed build events and CodeDeploy deployment information in the Jenkins Console Output.

   ![Console Output](https://user-images.githubusercontent.com/48589838/89986227-dd5a2180-dc99-11ea-95a5-15938ac49df1.png)

5. **Verification:** Confirm successful deployment using the provided ELBDNSName and ensure the web application is running as expected.

   ![Verification](https://user-images.githubusercontent.com/48589838/89986033-9409d200-dc99-11ea-883c-37f6a469e02c.png)

Feel free to follow the detailed steps and screenshots provided in this README to implement the CI/CD pipeline effectively.