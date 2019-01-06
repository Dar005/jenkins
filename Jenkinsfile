node {
    echo "JENKINS FILE"
   stage('checkout') { // for display purposes
      // Get some code from a GitHub repository
       checkout(
                              [$class: 'GitSCM',
                              branches: [[name: '*/master']],
                              doGenerateSubmoduleConfigurations: false,
                              extensions: [],
                              submoduleCfg: [],
                              userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
                  )

                   javac Student.java

   }
   stage('Build') {

        javac Student.java

   }
   stage('Test') {
        echo "Testing"
   }
}