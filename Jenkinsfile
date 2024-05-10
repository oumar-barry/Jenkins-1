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
            options {
                timestamps()
            }
            steps {
                echo "Coucou tout le monde "
                
            }
        }
    }
    
    

    
}