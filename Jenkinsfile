pipeline {
    agent any

    stages {
        stage('build'){
            steps {
                sh 'echo hello tout le monde > file.txt'
                archiveArtefacts(artefacts: '*.txt')
            }
        }

        stage('deploy'){
            steps {
                echo "Deploy to production "
            }
        }
    }
   
}