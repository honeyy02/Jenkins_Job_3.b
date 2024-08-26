pipeline {
    agent any

    stages {
        stage('Invoke Ansible Playbook') {
            steps {
                script {
                    // Run the Ansible playbook
                    sh 'ansible-playbook /etc/ansible/playbooks/copyJartoS3.yml'
                }
            }
        }
    }
}
