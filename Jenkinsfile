pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/Eman-Ali-E/Eman-ToCs-.git',
                branch: 'main'
            }
        }
        stage('Build Website') {
            steps {
                bat './hello.bat'
            }
        }
        stage('HTML Validation') {
            steps {
                echo 'Running HTML Validation...'
                bat 'echo HTML issues detected!'
            }
        }
    }
}
