pipeline {
    agent any

    tools {
        nodejs 'Node22'
    }

    stages {
        stage('build'){
            steps {
                sh 'npm -v'
                
            }
        }

        stage('deploy'){
            steps {
                echo "Deploy to production "
            }
        }
    }
   
}