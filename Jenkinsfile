pipeline {
    agent any 
     
        tools {
    maven 'Maven-3.8.9'
}
     
   
    stages{

        stage('Mavendefault') {
            steps{
                echo "hello Maven default version"

                sh 'mvn -version'
            }
        }

        stage('Mavencustom') {
            tools {
                jdk 'Java-17'
            }
            steps{
                echo "hello Maven section this is custom java version"

                sh 'mvn -version'
            }
        }
    }
}
