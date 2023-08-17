pipeline {
    agent any

    stages {
        stage('Testing connection') {
            steps {
                echo 'Start of Ansible ping'
                sh "ansible -m ping all"
                echo 'End of Ansible ping'
            }
        }
        stage('2-Test') {
            steps {
                echo 'Start of Stage Test'
                echo 'Testing............'
                echo 'End of Stage Testiong'
            }
        }
         stage('3-Deploy') {
            steps {
                echo 'Start of Stage Deploy'
                echo 'Deploying............'
                echo 'End of Stage Deploying'
            }
        }
    }
}

