node {
      stage ('Build and Test'){

            env.PATH = "${tool 'ant'}/bin:${env.PATH}"
            checkout(
                        [$class: 'GitSCM',
                        branches: [[name: '*/master']],
                        doGenerateSubmoduleConfigurations: false,
                        extensions: [],
                        submoduleCfg: [],
                        userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
            )
            bat 'ant build'

            echo "From jenkins file!!!....."


      }

 }
