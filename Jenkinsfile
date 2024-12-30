pipeline {
    agent any
    tools {
        maven 'Maven 3.8' // Use the name you configured in Global Tool Configuration
    }
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
