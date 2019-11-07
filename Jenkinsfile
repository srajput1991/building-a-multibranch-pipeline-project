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
                def scannerHome = tool 'SonarScanner 4.0';
                withSonarQubeEnv('Sonarqube') {
                     sh "${scannerHome}/bin/sonar-scanner"
                }
            }
        }
    }
}
