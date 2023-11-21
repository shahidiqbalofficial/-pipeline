pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
        stage('name') {
            steps {
                echo 'shahid iqbal'
            }
        }
        stage('class') {
            steps {
                echo 'Tocs Class'
            }
        }
    }
}