node {
  stage ('Build') {
        echo "JENKINSFILE>>>>>>>>>>>>>>>>>>>>>>>>>>>"
    git url:  'https://github.com/Dar005/jenkins/'

    withMaven(
        // Maven installation declared in the Jenkins "Global Tool Configuration"
        maven: 'Maven',
        // Maven settings.xml file defined with the Jenkins Config File Provider Plugin
        // Maven settings and global settings can also be defined in Jenkins Global Tools Configuration
        mavenLocalRepo: '.repository') {

      // Run the maven build
      bat "mvn clean install"

    } // withMaven will discover the generated Maven artifacts, JUnit Surefire & FailSafe & FindBugs reports...
  }

}