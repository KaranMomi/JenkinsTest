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
    success {
        slackSend channel: '#test',
                  color: 'good',
                  message: "The pipeline ${currentBuild.fullDisplayName} completed successfully."
    }
    }
}
