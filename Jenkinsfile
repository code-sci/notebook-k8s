node {

    stage('Pull source code') {
        git 'https://gitee.com/microshadow/notebook-k8s.git'

    }
    dir('notebook-service') {
        stage('Maven deploy'){
            sh '''
                mvn deploy -Dmaven.test.skip=true 
            '''
        }
    }
 }