# Building a CI/CD Pipeline in Jenkins

# Aim
Pipeline To Deploy The Web Application Into The Tomcat Server

# Task
1. Login into your Jenkins account. 
2. Build a new project and intiate build triggers.

Here is a Sample Pipelinescript To Deploy The Web Application Into The Tomcat Server

node
{
   //Mention the tools which have been configured
   
   def mavenhome= tool name:"*****"
   
   // Mention how to trigger the Pipeline and how many Builds must be there and so on 
   
   properties([buildDiscarder(logRotator(artifactDaysToKeepStr: 
   '', artifactNumToKeepStr: '5', daysToKeepStr: '
   ', numToKeepStr: '5')), pipelineTriggers([pollSCM('* * * * *')])])
   
   // Getting the code from the GitHub
   
   stage('checkout code'){
       git branch: 'development', credentialsId: '*******', url: '********'
   }

   //Building the code in to packages by using maven 
    
   stage('build'){ 
       sh "${mavenhome}/bin/mvn clean package"
       
   //Executing the code quality report by using SonarQube
      
   }
   stage('execute sonarqube package'){
        sh "${mavenhome}/bin/mvn clean sonar:sonar"

    //Uploading the package into nexus
    
   }
   stage('upload buildartifact'){
       sh "${mavenhome}/bin/mvn clean deploy"
    
    //Deploying th application into Tomcat
       
   }
   stage('tomcat'){
       sshagent(['**********']) {
       sh "scp -o  StrictHostKeyChecking=no target
       /maven-web-application.war ec2-user@*******:/opt/apache-tomcat-9.0.64/webapps/"
}
   }


3. Check if the pipeline was succesfuly built
4. Attached screenshots of successful completion in your screenshot directory of this lab
5. Perform clean up operations


# Guide:
Use video recording of class to help achieve each steps above.
Check out this guide https://www.geeksforgeeks.org/how-to-make-a-ci-cd-pipeline-in-jenkins/
