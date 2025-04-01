pipeline {
    agent any

    stages {
        stage('Install-pip-deps') {
            steps {
                echo 'Installing all required dependencies...'
                git url: 'https://github.com/mtararujs/python-greetings', branch: 'main'
                sh 'ls -la'  // Pēc izvēles: pārbauda failus
                sh 'pip install -r requirements.txt'
            }
        }
    }
}
