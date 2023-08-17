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
        stage('Configuration and Deployment') {
            steps {
                echo 'Start of Configuration and Deployment'
                sh "ansible-playbook playbook-php-istall.yml"
                echo 'End of Configuration and Deployment'
            }
        }
         stage('Configuration Testing') {
            steps {
                echo 'Start of Configuration Testing'
                sh "php -v"
                echo 'End of Configuration Testing'
            }
        }
    }
}

