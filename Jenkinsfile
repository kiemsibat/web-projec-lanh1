pipeline{
    agent any 
    stages {
         stage('SCM Checkout'){
            steps {    
                    git 'https://github.com/kiemsibat/web-projec-lanh1.git'
                }
            }
            
            stage('Executed Ansible'){
            steps {   
                ansiblePlaybook credentialsId: 'slave', disableHostKeyChecking: true, installation: 'ansible2', playbook: 'playbook.yml'
                }
            }
        }
    }