pipeline {
    agent none
    stages {
        stage('Build') {
                      steps {
                git url: 'https://github.com/bezracda/JavaScriptMasterHateThisTask.git'
                sh 'ls -la'
                echo 'Hello, Jenkins'
            }
        }
    }
    post { 
        always { 
            cleanWs()
        }
    }
}
