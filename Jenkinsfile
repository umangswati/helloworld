pipeline {
    agent any
    
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                echo "This is ${env.BUILD_NUMBER}"
                sh 'This is $WORKSPACE'
                sh 'This is $NODE_NAME'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
