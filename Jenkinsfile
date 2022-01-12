pipeline {
    agent master
    
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                echo "This is ${env.BUILD_NUMBER}"
               
                echo "This is ${env.NODE_NAME}"
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
