pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Running build..'
            }
        }
        stage('images') {
            steps {
                echo 'Creating images'
            }
        }
        stage('files path') {
            steps {
                echo 'files path'
            }
        }
        stage('final stage') {
            steps {
                echo 'done'
            }
        }
    }
    post {
    always {
        slackSend "started ${env.JOB_NAME} ${env.BUILD_NUMBER} (<${env.BUILD_URL}|Open>)"
    }
    }
}
