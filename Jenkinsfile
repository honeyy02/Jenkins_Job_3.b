pipeline {
    agent any

    stages {
        stage('Invoke Ansible Playbook') {
            steps {
                script {
                    // Run the Ansible playbook
                    sh 'ansible-playbook copyJartoS3.yml'
                }
            }
        }
    }
}
