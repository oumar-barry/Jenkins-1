pipeline {
    agent any

    options {
        timeout(time: 1, unit: 'HOURS')
    }

    triggers{
        cron('* * * * *')
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
    
    

    
}