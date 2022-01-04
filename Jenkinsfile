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
                sh "sudo su - mqm ./create_qmgr.pl"
            }
        }
        
        stage ('Deploy') { 
            steps {
                echo 'Deploying the job'
                sh "sudo su - mqm `strmqm TEST1`"
            }
        
        }
        
 
    }           
 }
