pipeline { 
agent any 
    stages { 
        stage ('Build') { 
            steps {
                echo 'Building the job'
            }
 
        }
        stage ('Test') { 
            steps {
                echo 'Testing the job'
                sh "whoami"
                sh "./create_qmgr.pl"
            }
        }
        
        stage ('Deploy') { 
            steps {
                echo 'Deploying the job'
            }
        
        }
        
 
    }           
 }
