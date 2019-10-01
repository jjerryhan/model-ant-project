pipeline {
    stages {
        stage('build-develop') {
            environment {
                servertype='uat'
            }
            steps {
                withAnt(installation: 'Ant 1.10.6', jdk: 'JDK 1.8.0_221') {
                    bat 'ant package -Dservertype=develope'
                }
            }
        }
        stage('dist') {
            steps {
                echo 'copy to target location'
            }
        }
        stage('deploy') {
            steps {
                echo 'restart was'
            }
        }
    }
}
