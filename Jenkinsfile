pipeline {
    agent any
    stages{
        stage (build) {
            steps{

            echo "This is a build stage"
            sh "hostname-i"
        }
        }

      stage (groovy script) {
        steps {
            script{
                def course = "k8s"

                if (course == "k8s") {

                println "Thanks for enrolling ${course} course"
                }
                else {
                println "Do enroll into ${course} course"
                }
            }

        }

      }
    }

}
