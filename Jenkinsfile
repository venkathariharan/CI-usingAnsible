pipeline {
    agent any
    
    
     
    stages {
      stage('checkout') {
           steps {
             
                git branch: 'master', url: 'https://github.com/venkathariharan/CI-usingAnsible.git'
             
          }
        }
        
 
        
         stage('Code build') {
           steps {
             
                //sh 'mvn package'             
          }
        }
        
      stage('Ansible Deploy') {
             
            steps {
                 
           //sh "ansible-playbook main.yml -i inventories/dev/hosts --user jenkins --key-file ~/.ssh/id_rsa"
}
}
        
        
    }
}
