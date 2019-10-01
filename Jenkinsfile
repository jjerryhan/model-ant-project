======jenkins file=================
pipeline {
    environment {
        java_7_runtime_lib=‘E:/alm/java/jdk1.7.0_80/jre/lib'
        javac_7 = 'E:/alm/java/jdk1.7.0_80/bin/javac'
    }
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
