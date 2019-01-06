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
        echo "IN BUILD"
        javac \Program Files (x86)\Jenkins\workspace\devops

   }
   stage('Test') {
        "IN TESTING"
        echo "Testing"
   }
}