pipeline{

    stages{

        stage('checkout'){
               checkout(
                                    [$class: 'GitSCM',
                                    branches: [[name: '*/master']],
                                    doGenerateSubmoduleConfigurations: false,
                                    extensions: [],
                                    submoduleCfg: [],
                                    userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
                        )
        }
        stage('build'){
               bat 'mvn clean install'
        }
        echo "FUCK THIS........"

    }


}