pipeline {
    agent any
    stages {
        stage('build'){
            steps{
                echo "*** Building the artifact***"
            }
     
       }
      stage('sonar'){
            steps{
                echo "*** Verifying sonar***"
            }
     
       }
      stage('Docker'){
            steps{
                echo "*** Docker pushing***"
            }
     
       }

       stage('Docker'){
            steps{
                echo "*** Deploy to Dev***"
            }
     
       }

       stage('Docker'){
            steps{
                echo "*** Deploy to Test***"
            }
     
       }
       stage('Docker'){
         input {
            message "Are you sure you want to deploy to prod"
            ok "yes"
            Submitter "swathitdevops,sreuser"

         }
            steps{
                echo "*** Deploy to Prod***"
            }
     
       }
