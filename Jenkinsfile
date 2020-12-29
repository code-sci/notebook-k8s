node {
	def mvnHome
    stage('Pull source code') {
        git 'https://github.com/code-sci/notebook-k8s.git'
		mvnHome = tool 'maven'
    }
    dir('notebook-service') {
        stage('Maven build and Unit Test'){
            sh '''
                mvn deploy

            '''

        }

       

    }

 }