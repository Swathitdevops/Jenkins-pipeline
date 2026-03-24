pipeline {
    agent {
        label 'Docker-Slave'
        }
    stages{
        stage(docker version) {
            steps{
                sh "docker --version"
            }
        }

        stage(Docker Images) {
            
            steps {
                sh " docker image"       
                  }
        }

        stage(hostname){
            steps {
               sh 'hostname -i'
            }
        }
            
    }
    
}
