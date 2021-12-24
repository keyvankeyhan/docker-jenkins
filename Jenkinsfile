pipeline {
    agent any
    stages {
        stage('Download Jenkinsfile') {
            steps {
                echo 'Get Jenkinsfile from GitHub'
                echo "Checkout directory is ${GIT_CHECKOUT_DIR}"
                //git 'https://github.com/keyvankeyhan/cicd-test'
            }
        }
        stage('Build from Jenkinsfile') {
            steps {
                echo 'Build Application from Jenkinsfile'
                sh './build.sh'
            }
        }
        stage('Test from Jenkinsfile') {
            steps {
                echo 'Run script test.sh from Jenkinsfile'
                sh './test.sh'
            }
        }
    }
}