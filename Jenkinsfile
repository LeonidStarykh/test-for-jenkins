pipeline {
    agent any

    environment {
        PROJECT_NAME = "ISPRAS Proj"
        OWNER_NAME = "Leo Star"
    }
    
    stages {
        stage('1-build') {
            steps {
                echo 'Start of stage 1-build'
                echo 'Building...'
                echo 'End of stage 1-build'
            }
        }
        stage('2-test') {
            steps {
                echo 'Start of stage 2-test'
                echo 'Testing...'
                sh "ls -al"
                echo "Hello, ${OWNER_NAME}"
                echo "Project name is , ${PROJECT_NAME}"
                echo 'End of stage 2-test'
            }
        }
        stage('3-deploy') {
            steps {
                echo 'Start of stage 3-deploy'
                echo 'Deploying...'
                sh '''
                    echo "text1"
                    echo "test2"
                '''
                sh "python3 --version"
                echo 'End of stage 3-deploy'
            }
        }
        stage('4-after') {
            steps {
                echo 'GOTOVO from GitHub pipeline'
            }
        }
    }
}
