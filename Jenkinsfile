    pipeline {
        agent {
            docker {
                image 'node:22-alpine'
                args '-p 3000:3000 -u root:root'
            }
        }
        environment {
                CI = 'true'
            }

        stages {
            
            stage('Install Dependencies') {
                steps {
                    sh '''
                        npm install
                    '''
                }
            }

            
        
            
            stage('Deploy') {
                steps {
                    sh '''
                       npm start
                        
                        echo "Application deployed at http://localhost:3000"
                    '''
                }
            }
        }
    }