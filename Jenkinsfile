node {
   checkout(
        [$class: 'GitSCM',
        branches: [[name: '*/master']],
        doGenerateSubmoduleConfigurations: false,
        extensions: [],
        submoduleCfg: [],
        userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
   )
}
        stage('Build'){
        echo "Inside build stage"
            step{
                bat 'make'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            }
        }

   echo "From jenkins file!!!....."


