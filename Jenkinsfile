node {
      stage ('Build and Test'){

            env.PATH = "${tool 'Ant'}/bin:${env.PATH}"
            checkout(
                        [$class: 'GitSCM',
                        branches: [[name: '*/master']],
                        doGenerateSubmoduleConfigurations: false,
                        extensions: [],
                        submoduleCfg: [],
                        userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
            )

            echo "From jenkins file!!!....."

      }
      bat 'build'
 }
