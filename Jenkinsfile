pipeline {
    agent any

    parameters {
        booleanParam(name: 'DEPLOY_TO', defaultValue: 'false', description: 'Deploy to production ? ')
    }
    
    stages {
        stage('build'){
            steps {
                echo "Building the app"
            }
        }

        stage('deploy'){
            when {
                branch 'prod'
                expression {DEPLOY_TO}
            }
            
            steps {
                echo "App going to production"
            }
        }
    }
    
    

    
}