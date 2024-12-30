pipeline {
    agent any
    stages {
        stage('Check Maven Installation') {
            steps {
                script {
                    // Check if Maven is installed
                    try {
                        sh 'mvn -version'
                    } catch (Exception e) {
                        error "Maven is not installed or not properly configured on this Jenkins instance."
                    }
                }
            }
        }
    }
}
