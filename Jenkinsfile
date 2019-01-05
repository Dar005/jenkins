node {
agent any

       checkout(
            [$class: 'GitSCM',
            branches: [[name: '*/master']],
            doGenerateSubmoduleConfigurations: false,
            extensions: [],
            submoduleCfg: [],
            userRemoteConfigs: [[url: 'https://github.com/Dar005/jenkins/']]]
       )

       build 'DevOpsJenkins'

       echo "From jenkins file!!!....."


 }
