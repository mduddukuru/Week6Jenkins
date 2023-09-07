pipeline{
    agent any 
    
    stages {
        stage('Build'){
            steps{
                echo "Build an automation tool to compile and package code"
                echo "Build the code using Maven"
            }
        }
        stage('Test'){
            steps{
                echo "Perform unit testing with Mocha"
                echo "Perform integration testing with Mockito"
            }
        }
        stage('Code'){
            steps{
                echo "integrate the code via CheckStyle using Jenkins"
            }
        }
        stage('Security Scan'){
            steps{
                echo "perform security scan using WireShark"
            }
        }
        stage('Deploy to Staging'){
            steps{
              echo "deploy the application to a staging server by using AWS EC2"
        }
        }
        stage('Integration Tests on Staging'){
            steps {
                echo "run integration testing with Mockito"
            }
        }
        stage('Deploy to Production'){
            steps {
                echo "deploy the application to a production server via AWS EC2"
            }
        }
    }
    post {
        success {
        mail to: "mduddukuru@gmail.com"
        subject: "Build Status Email - Week 6"
        body: "The build was successful"
        }
       
    }
}