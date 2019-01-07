pipeline {
    agent any

   stages{
        stage('checkout') { // for display purposes

            steps{
                echo "In CHECKOUT"
                // Get some code from a GitHub repository
                git url: 'https://github.com/Dar005/jenkins/'
            }

        }

            stage('Build') {
                steps{
                    echo "IN BUILD FILE"
                    bat 'javac -cp junit-4.12.jar;hamcrest-core-1.3.jar;. Student.java StudentTest.java'

                    echo "EXIT BUILD"
                }

        }

        stage('Test') {
            steps{
                   echo "Testing"
                   bat 'java -cp junit-4.12.jar;hamcrest-core-1.3.jar;. org.junit.runner.JUnitCore StudentTest'
                   echo "TESTS FINISHED....."
            }
        }
   }
}