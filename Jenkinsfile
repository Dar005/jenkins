node {
        echo "JENKINSFILE>>>>>>>>>>>>>>>>>>>>>>>>>>>"
        checkout(
                           [$class: 'GitSCM',
                           branches: [[name: '*/master']],
                           doGenerateSubmoduleConfigurations: false,
                           extensions: [],
                           submoduleCfg: [],
                           userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
        )

        stage('Build') {
            step {
                echo 'Building..'
            }
        }
        stage('Test') {
            step {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            step {
                echo 'Deploying....'
            }
        }
}