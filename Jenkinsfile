pipeline {
    agent {
        label 'dev-slave'
        }
    stages{
        stage(build) {
            steps{
                echo "Hello world"
            }
        }

        stage(test) {
            steps {
                echo "Testing"
            }
        }

        stage(hostname){
            steps {
               sh 'hostname -i'
            }
        }
            
    }
    
}
