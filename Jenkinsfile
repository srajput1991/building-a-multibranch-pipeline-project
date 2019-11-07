pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
        stage ("scan-publish-sonar"){
            steps {
                withSonarQubeEnv('Sonarqube') {
                    
                }
            }
        }
    }
}
