pipeline{
    agent any
stages{
    stage('Dry Run Playbook'){
       steps{
        sh '''
           hostname
ansible-playbook install.yaml -e ansible_user=centos -e ansible_password=DevOps321-e ENV=dev
        
        '''
 }
    }
}
}