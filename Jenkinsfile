node {
    echo "JENKINS FILE"
   stage('checkout') { // for display purposes

   echo "In CHECKOUT"
      // Get some code from a GitHub repository
       checkout(
                              [$class: 'GitSCM',
                              branches: [[name: '*/master']],
                              doGenerateSubmoduleConfigurations: false,
                              extensions: [],
                              submoduleCfg: [],
                              userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
                  )


   }
   stage('Build') {
        echo "IN BUILD FILE"
        javac -classpath C:/jars/junit-4.12.jar;C:/jars/hamcrest-core-1.3.jar;C:/Program_Files_(x86)/Jenkins/Jenkins/workspace/Test1/;. Student.java StudentTest.java
        echo "EXIT BUILD"
   }
   stage('Test') {
        "IN TESTING"
        echo "Testing"
        java -cp C:/jars/junit-4.12.jar;C:/jars/hamcrest-core-1.3.jar;. org.junit.runner.JUnitCore StudentTest
        echo "TESTS FINISHED....."
   }
}
