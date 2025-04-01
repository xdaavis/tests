pipeline {
    agent any

    stages {
        stage('Install-pip-deps') {
            steps {
                echo 'Installing all required dependencies...'
                git url: 'https://github.com/mtararujs/python-greetings', branch: 'main'
                dir("${WORKSPACE}") { // Pievienots dir bloks
                    bat 'dir'  // Windows: pārbauda failus
                    bat 'pip install -r requirements.txt'
                }
            }
        }
    }
}
