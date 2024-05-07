pipeline {
    agent {
        docker {
            image 'node:21-alpine'
        }
    }

    stages {
        stage('build'){
            steps {
                sh 'node -v '
            }
        }
    }
    
    post {
        success {
            echo 'success'
        }
        always {
            echo 'always'
        }
    }

    
}