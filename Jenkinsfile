pipeline {
node  {
  	stage('SCM checkout'){
		git 'https://github.com/sivaprasad9/githubaug04.git'
	}
	
	
}
	
	 agent any
    tools {
        maven 'Maven_3.6.3' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }

          stage('deployment stage') {
              steps {
                bat "mvn deploy"
        }
    }

  }

	
}

