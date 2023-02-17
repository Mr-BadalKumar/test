pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'building the application'
            }
        }
        

        stage('Docker Build') {
    	agent any
      steps {
      	sh 'docker build -t badal773/jenkins-docker  .'
             }
                                }
        stage('Test') { 
            steps {
                 echo 'testing  the application'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'deploying the application'
            }
        }
    }
}
