pipeline {
    agent {
        label 'Docker-Slave'
        }
    stages{
        stage(Dockerversion) {
            steps{
                sh "docker --version"
            }
        }

        stage(DockerImages) {
            
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
