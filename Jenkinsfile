pipeline {
    agent any

    stages {
        stage('build'){
            steps {
                sh 'echo hello tout le monde > file.txt'
                archiveArtifacts(artifacts: '*.txt')
            }
        }

        stage('deploy'){
            steps {
                echo "Deploy to production "
            }
        }
    }
   
}