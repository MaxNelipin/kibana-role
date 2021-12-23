pipeline {
    agent {
        label 'docker'
    }
    stages {

            stage ('Get chekout'){
                steps {
                         ws('kibana-role') {
                        git credentialsId: 'c8f2dc93-57e2-4187-9669-75e746f5a9e1', url: 'git@github.com:MaxNelipin/kibana-role.git'
                         }

                }
            }
            stage ('Install requiments'){
                steps {
                    sh "pip3 install -r test-requirements.txt"
                }
            }
            stage ('molecule test'){
                    steps {
                        ws('kibana-role') {
                        sh 'molecule test'
                        }
                    }
            }

    }
}