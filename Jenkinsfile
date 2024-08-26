pipeline {
    agent any
    environment {
        AWS_CREDENTIALS = credentials('aws-credentials') // The ID of the AWS credentials you created
    }

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
