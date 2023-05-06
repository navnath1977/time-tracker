pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
        stage('Test') {
            steps {
                echo 'Test App'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
    }
    post
    {
        always
        {
            emailext body: 'Your Pipeline was successful', subject: 'Pipeline Status', to: 'drnavnathkale@gmail.com'
        }
    }
}
