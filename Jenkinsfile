    pipeline {
        agent any

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