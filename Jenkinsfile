pipeline {
    agent any
    
    
     
    stages {
      stage('checkout') {
           steps {
             
                git branch: 'master', url: 'https://github.com/venkathariharan/CI-usingAnsible.git'
             
          }
        }
        
       
        
         stage('Execute Maven') {
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
