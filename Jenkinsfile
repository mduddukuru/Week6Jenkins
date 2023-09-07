pipeline{
    agent any 
    environment {
        PRODUCTION_ENVIRONMENT = "mduddukuru"
    }
    stages {
        stage('Build'){
            steps{
                echo "fetch the source code from the directory path specified by the environment variable"
                echo "compile the code and generate any necessary artifacts"
            }
        }
        stage('Test'){
            steps{
                echo "unit tests"
                echo "integration tests"
            }
        }
        stage('Code'){
            steps{
                echo "check the quality of the code"
            }
        }
        stage('Deploy'){
            steps{
                echo "deploy the application to a testing environment specified by the environment variable"
            }
        }
        stage('Approval'){
            steps{
              echo "Approval"
            sleep 10  
        }
        }
        stage('Deploy to Production'){
            steps {
                echo "Deploying code to the production environment ${PRODUCTION_ENVIRONMENT}"
            }
        }
    }
}