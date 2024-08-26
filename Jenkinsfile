pipeline {
    agent any

    stages {
        stage('Invoke Ansible Playbook') {
            steps {
                script {
                    withCredentials([[$class: 'AmazonWebServicesCredentialsBinding', credentialsId: 'aws_credentials']]) {
                // Run your Ansible playbook
                sh '''
                ansible-playbook copyJarToS3.yml
                '''
                }   

                }
            }
        }
    }
}
