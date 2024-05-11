pipeline {
    agent any

    parameters {
        booleanParam(name: 'DEPLOY_TO', defaultValue: 'false', description: 'Deploy to production ? ')
    }
    
    stages {
        stage('build'){
            parallel {
                stage('build frontend'){
                    steps {
                        echo "Building frontend"
                    }
                }

                stage('build backend'){
                    steps {
                        echo "Building backend"
                    }
                }
            }
        }

        stage('deploy'){
            when {
                branch 'main'
                expression {DEPLOY_TO}
            }
            
            steps {
                echo "App going to production"
            }
        }
    }
    
    

    
}