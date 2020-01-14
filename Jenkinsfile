node {
	stage('SCM checkout'){
		git 'https://github.com/sivaprasad9/githubaug04.git'
	}
	stage('compile-package'){
		def mvnHome = tool name: 'M3', type: 'maven'
		 bat "mvn clean install"
	}
	
}
