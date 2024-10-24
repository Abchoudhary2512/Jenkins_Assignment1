pipeline {
    agent any  // This allows the job to run on any available agent

    stages {
        stage('Check Node and npm Version') {
            steps {
                bat "node --version"  // Check Node.js version
                bat "npm --version"   // Check npm version
            }
        }
    }
}
