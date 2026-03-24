
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "*** Building the artifact ***"
            }
        }

        stage('Sonar') {
            steps {
                echo "*** Verifying Sonar ***"
            }
        }

        stage('Docker Push') {
            steps {
                echo "*** Docker pushing ***"
            }
        }

        stage('Dev') {
            steps {
                echo "*** Deploy to Dev ***"
            }
        }

        stage('Test') {
            steps {
                echo "*** Deploy to Test ***"
            }
        }

        stage('Prod') {
            options {
                timeout(time: 300, unit: 'SECONDS') // timeout in seconds
            }
            input {
                message "Are you sure you want to deploy to Prod?"
                ok "Yes"
                submitter "swathitdevops,sreuser"
            }
            steps {
                echo "*** Deploy to Prod ***"
            }
        }
    }

    post {
        always {
            echo "*** This will run regardless of success or failure ***"
        }

        success {
            echo "*** This will run once the build is successful ***"
        }

        failure {
            echo "*** This will run if the job fails ***"
        }
    }
}
