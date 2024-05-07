pipeline {
    agent any

    options {
        timeout(time: 1, unit: 'HOURS')
    }

    parameters {
        text(name: 'NAME', defaultValue: 'Barry', description: 'name field')
        string(name: 'STRING', defaultValue: 'a long text', description: 'text field ')
        booleanParam(name: 'BOOLEAN', defaultValue: 'true', description: 'boolean field' )
        choice(name: 'CHOICE', choices: ['one','two', 'tree'], description: 'choice field')
        password(name: 'PASSWORD', description: 'Password field ')
    }
    stages {
        stage('build'){
            options {
                timestamps()
            }
            steps {
                echo "Coucou tout le monde "
                echo "NAME: ${NAME}"
                echo "STRING: ${STRING}"
                echo "BOOLEAN: ${BOOLEAN}"
                echo "CHOICE: ${CHOICE}"
                echo "PASSWORD: ${PASSWORD}"
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