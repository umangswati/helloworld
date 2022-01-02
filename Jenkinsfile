pipeline {
  agent any 
      stages {
         stage('Build') { 
           steps {
              sh 'Building the job' 
             }
      }
        stage('Test'){
           steps {
              sh 'Testing the job'
              
           }
      }
        stage('Deploy') {
           steps {
             sh 'Deploying the job'
            }
        }
  }
}

