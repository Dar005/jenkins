node {
    echo "JENKINS FILE"
   stage('checkout') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/Dar005/jenkins.git'

   }
   stage('Build') {

        javac Student.java

   }
   stage('Test') {
        echo "Testing"
   }
}