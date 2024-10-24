pipeline {
    agent any  // Use 'any' to run on any available agent

    stages {
        stage('Check Node.js and npm Versions') {
            steps {
                // Check Node.js version
                script {
                    def nodeVersion = bat(script: 'node --version', returnStdout: true).trim()
                    echo "Node.js version: ${nodeVersion}"
                }
                
                // Check npm version
                script {
                    def npmVersion = bat(script: 'npm --version', returnStdout: true).trim()
                    echo "npm version: ${npmVersion}"
                }
            }
        }
    }
}
