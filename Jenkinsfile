pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                snDevOpsStep()
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                snDevOpsStep()
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                snDevOpsStep()
                snDevOpsChange()
                echo 'Deploying....'
            }
        }
    }
}
