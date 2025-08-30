pipeline {
    agent { label 'jenkins-agent1' }
    tools {
        git 'Git'
    }

    stages {
        stage('clean ws') {
            steps {
                cleanWs()
            }
        }
        stage('Git clone scm') {
            steps {
                git 'https://github.com/khanarshad23/nodejs-on-ec2-youtube.git'
            }
        }
        stage('npm install') {
            steps {
                sh 'npm install'
            }
        }                
    }
}
