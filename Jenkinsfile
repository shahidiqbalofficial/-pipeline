pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/shahidiqbalofficial/-pipeline.git', branch: 'master'
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
                echo 'Deploying..'
                sshPublisher(
                    publishers: [
                        sshPublisherDesc(
                            configName: 'ShahidSSH',
                            transfers: [sshTransfer(sourceFiles: '**/*', remoteDirectory: '/home/myapp')],
                        )
                    ]
                )
            }
        }
    }
}
