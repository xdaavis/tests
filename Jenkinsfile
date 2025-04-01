pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: '<your_repository_url>', branch: 'main' // Aizstāj ar savu URL un zaru
            }
        }
        stage('Execute Script') {
            steps {
                echo "Executing script"
                sh './script.sh'  // Linux/Unix
                //bat 'script.bat' // Windows
            }
        }
    }
}
