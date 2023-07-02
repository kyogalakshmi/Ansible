pipeline{
    agent {
        node{
            label 'WS'
        }
    }
    environment{
        ENV_URL ="pipeline.ggogle.com"
        SSHCRED =credentials('SSH_CRED')
    }
    stages{
    stage('Dry Run Playbook'){
        sh '''
ansible-playbook install.yaml -e ansible_user=centos -e ansible_password=DevOps321-e ENV=dev
        echo hostname
        '''
    }
}
}