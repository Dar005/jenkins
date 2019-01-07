pipeline {
    agent any

   stages{
        stage('checkout') { // for display purposes

            step{
                echo "In CHECKOUT"
                // Get some code from a GitHub repository
                git url: 'https://github.com/Dar005/jenkins/'
            }

        }

            stage('Build') {
                step{
                    echo "IN BUILD FILE"
                    bat 'javac -cp junit-4.12.jar;hamcrest-core-1.3.jar;. Student.java StudentTest.java'

                    echo "EXIT BUILD"
                }

        }

        stage('Test') {
            step{
                  "IN TESTING"
                   echo "Testing"
                   bat 'java -cp junit-4.12.jar;hamcrest-core-1.3.jar;. org.junit.runner.JUnitCore StudentTest'
                   echo "TESTS FINISHED....."
            }
        }
   }
}
