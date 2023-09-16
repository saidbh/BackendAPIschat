pipeline {
    agent any
    stages {
        stage("Clone Git Repository") {
            steps {
               dir("Backend") {
                git(
                    url: "https://gitlab.com/w814/my-awesome-mobile-app.git",
                    branch: "developer",
                    changelog: true,
                    poll: true
                )
                }
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}