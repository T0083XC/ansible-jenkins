pipeline {
    agent any
    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/T0083XC/ansible-jenkins.git'
            }
        }
        stage('Run Ansible Playbook') {
            steps {
                sh 'ansible-playbook -i hosts install_apache.yml'
            }
        }
    }
}
