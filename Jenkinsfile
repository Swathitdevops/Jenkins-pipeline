pipeline {
    agent any 
     
        tools {
    maven 'Maven-3.8.9'
}
     
   
    stages{

        stage('Maven') {
            steps{
                echo "helPrint Maven version"

                sh 'mvn -version'
            }
        }
    }
}
