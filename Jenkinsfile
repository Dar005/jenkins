node {
      stage ('Build and Test'){

            env.PATH = "${tool 'Maven'}/bin:${env.PATH}"
            checkout(
                        [$class: 'GitSCM',
                        branches: [[name: '*/master']],
                        doGenerateSubmoduleConfigurations: false,
                        extensions: [],
                        submoduleCfg: [],
                        userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
            )

            withAnt(installation: 'Ant') {
               bat "maven build"
            }

            echo "From jenkins file!!!....."

      }

 }
