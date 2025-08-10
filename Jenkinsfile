pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/6nik6hil6/RobotPractice.git'
            }
        }
        stage('Install Requirements') {
            steps {
                bat '"C:\\Users\\nikhi\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pip install -r requirements.txt'
            }
        }
        stage('Run Tests') {
            steps {
                bat '"C:\\Users\\nikhi\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m robot TestCodes'
            }
        }
    }
}
