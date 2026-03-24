pipeline {
    agent any
    stages {
        stage('Build')  {
            steps{

                echo "*** Building the application ***"

            }
        }
    }

    post {
        always {
            echo "*** This will run either success or Failure"
        }

        success {
            echo "*** This will run once the buils is success"
        }

        failure {
            echo "***This will run if the job fails***"
        }
    }
}
