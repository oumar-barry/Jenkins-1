pipeline {
    agent any

    stages {
        stage('build'){
            steps {
                sh "Build complete"
            }
        }

        stage('deploy'){
            steps {
                echo "Deploy to production "
            }
        }
    }

    post {
        success {
            emailext(to: 'alphaoumareclipse@gmail.com', body: $DEFAULT_CONTENT, subject: $DEFAULT_SUBJECT)
        }
    }
   
}