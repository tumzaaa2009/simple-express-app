pipeline {
    
    agent any 
 
    stages {
 
        stage('npm install'){
            steps {
                echo 'install'
                echo '******************************'  
                echo "build number : ${env.BUILD_NUMBER}"
            }
        }
 
        stage('npm run start') {
            steps {
                echo 'run start'
                echo '******************************'
            }
        }
 
    
    }
}
