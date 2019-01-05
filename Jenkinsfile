node{

    stages{

        stage('build'){


               checkout(
                                    [$class: 'GitSCM',
                                    branches: [[name: '*/master']],
                                    doGenerateSubmoduleConfigurations: false,
                                    extensions: [],
                                    submoduleCfg: [],
                                    userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
               )
            
            bat 'mvn clean install'
        }
        echo "FUCK THIS........"

    }


}