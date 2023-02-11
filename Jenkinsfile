pipeline {
    agent any
    stages {
        stage('Build') {
                      steps {
                git url: 'https://github.com/bezracda/JavaScriptMasterHateThisTask.git'
                sh './mvnw package'
                archiveArtifacts artifacts: 'target/*.jar', fingerprint: true
            }
        }
    }
    post { 
        always { 
            cleanWs()
        }
    }
}
