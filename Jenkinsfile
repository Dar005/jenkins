node {
  stage ('Build') {

    git url: 'https://github.com/Dar005/jenkins.git'
      env.PATH = "${tool 'Maven'}/bin:${env.PATH}"

      // Run the maven build
      bat "mvn clean install"

    echo "Please work its been 5 days......"
  }
}