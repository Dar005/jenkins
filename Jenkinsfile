pipeline {
    agent any


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




    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
      }
    }
}