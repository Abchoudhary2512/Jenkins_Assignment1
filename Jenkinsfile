    pipeline {
        agent any

      

        stages {
            
            stage('Install Dependencies') {
                steps {
                    bat '''
                        npm install
                    '''
                }
            }

            
        
            
            stage('Deploy') {
                steps {
                    bat '''
                       npm start
                        
                        echo "Application deployed at http://localhost:3000"
                    '''
                }
            }
        }
    }