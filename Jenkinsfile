pipeline {
    agent any
    
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                echo "This is ${env.BUILD_NUMBER}"
                sh 'ansible --version'
                sh 'ansible-playbook first.yml'
               
                echo "This is ${env.NODE_NAME}"
            }
        }
    }
    post { 
        always { 
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
  
        }
    }
}
