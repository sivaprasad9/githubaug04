pipeline {
 agent any
    tools {
        maven 'M3' 
    }
    stages {
	
       stage('SCM checkout'){
	     steps {
		git 'https://github.com/sivaprasad9/githubaug04.git'
	     }
	}    
        stage('Compile stage') {
            steps {
                echo "${env.WORKSPACE}"
                bat  """
                
                cd  "${env.WORKSPACE}/enq/sam/com.enq
                mvn clean compile 
                
                """
                
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

