pipeline{
    agent {
        node{
            label 'WS'
        }
    }
    
stages{
    stage('Dry Run Playbook'){
       steps{
        sh '''
ansible-playbook install.yaml -e ansible_user=centos -e ansible_password=DevOps321-e ENV=dev
        echo hostname
        '''
 }
    }
}
}