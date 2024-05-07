pipeline {
    agent any

    options {
        timeout(time: 1, unit: 'HOURS')
    }
    stages {
        stage('build'){
            options {
                timestamps()
            }
            steps {
                echo "Coucou tout le monde "
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