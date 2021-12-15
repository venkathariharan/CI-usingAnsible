pipeline {
    agent any
    
    
     
    stages {
      stage('checkout') {
           steps {
             
                git branch: 'master', url: 'https://github.com/venkathariharan/CI-usingAnsible.git'
             
          }
        }
        
       stage('Terraform Infrastructure deployment') {
           steps {
             
               sh "echo execute Terraform Infrastructure deployment"             
          }
        }
        
         stage('Code Build') {
           steps {
             
               sh "echo execute code build"             
          }
        }
        
      stage('Ansible Deploy') {
             
            steps {
               sh "echo Ansible deploy"  
           //sh "ansible-playbook main.yml -i inventories/dev/hosts --user jenkins --key-file ~/.ssh/id_rsa"
}
}
        
        
    }
}
