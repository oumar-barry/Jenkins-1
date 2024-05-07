pipeline {
    agent any

    environment{
        MY_VAR = "12345"
    }
    stages {
        stage('build'){
            steps{
                echo "BRANCH_NAME: ${env.BRANCH_NAME}"
                echo "BRANCH_IS_PRIMARY: ${env.BRANCH_IS_PRIAMRY}"
                echo "CI: ${env.CI}"
                echo "BUILD_NUMBER: ${env.BUILD_NUIMBER}"
                echo "JENKINS_URL: ${JENKINS_URL}"
                echo "MY_VAR: ${env.MY_VAR}"
            }
        }

        

    }
}