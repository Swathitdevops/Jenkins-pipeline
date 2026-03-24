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

       stage('Dev'){
            steps{
                echo "*** Deploy to Dev***"
            }
     
       }

       stage('Test'){
            steps{
                echo "*** Deploy to Test***"
            }
     
       }
       stage('Prod'){
        options {
            timeout(time:300, unit: SECONDS)
        }
         input {
            message "Are you sure you want to deploy to prod"
            ok "yes"
            submitter "swathitdevops,sreuser"

         }
            steps{
                echo "*** Deploy to Prod***"
            }
     
       }



    }
    
}
