node {
    echo "JENKINSFILE>>>>>>>>>>>>>>>>>>>>>>>>>>>"
    checkout(
        git url:  'https://github.com/Dar005/jenkins/'
    )
    pipeline {
    Sagent any

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