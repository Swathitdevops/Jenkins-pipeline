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
            agent {
                label  'app-slave'
            }
            steps {
                echo "print hte hostname "
                sh 'hostname -i'        
                  }
        }

        stage(hostname){
            steps {
               sh 'hostname -i'
            }
        }
            
    }
    
}
