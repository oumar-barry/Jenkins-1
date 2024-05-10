pipeline {
    agent any

    options {
        timeout(time: 1, unit: 'HOURS')
    }

    triggers{
        pollSCM('* * * * *')
    }

    
    stages {
        stage('build'){
            
            steps {
                echo "Coucou tout le monde "
                echo "Another modification"
                echo "This poll is working"
                
            }
        }

        stage('deploy'){
            input {
                message 'Would you like to deploy to production'
                ok 'deploy now'
                submitter 'admin,devops'
                parameters { 
                    string(name: 'VERSION', defaultValue: 'latest', description: 'The version of the deployed app ')
                }
            }

            
            steps {
                echo "App going to production"
                echo "VERSION: ${VERSION}"
                
            }
        }
    }
    
    

    
}