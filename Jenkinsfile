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
                    javac -cp "C:/jars/junit-4.12.jar;C:/jars/hamcrest-core-1.3.jar";"C:/Program_Files_(x86)/Jenkins/Jenkins/workspace/Test1/";. Student.java StudentTest.java
                    echo "EXIT BUILD"
                }

        }

        stage('Test') {
            step{
                  "IN TESTING"
                   echo "Testing"
                   java -cp "C:/jars/junit-4.12.jar";"C:/jars/hamcrest-core-1.3.jar";. org.junit.runner.JUnitCore StudentTest
                   echo "TESTS FINISHED....."
            }
        }
   }
}
