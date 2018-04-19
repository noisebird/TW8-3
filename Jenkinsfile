
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'gradlew build --info'
            }
        }
        stage('Test') {
            steps {
                sh 'gradlew test --info'
            }
        }

    }
}
