pipeline {
    agent any

    stages {
        stage('build and test'){
            matrix {
                axes {
                    axis {
                        name 'PLATFORM'
                        values 'Linux','Mac OS', 'Windows'
                    }
                    axis {
                        name 'BROWSER'
                        values 'Brave', 'Chrome', 'Firefox'
                    }
                }
                stages{
                    stage('build'){
                        steps {
                            echo "Building for ${PLATFORM} - ${BROWSER}"
                        }
                    }

                    stage('test'){
                        steps {
                            echo "Testing for ${PLATFORM} - ${BROWSER}"
                        }
                    }
                }
            }

            
        }   
        
        stage('deploy'){
            steps {
                echo "Deploying the app to production "
            }       
        }
    }
}