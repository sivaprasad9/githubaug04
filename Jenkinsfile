node  {
  	stage('SCM checkout'){
		git 'https://github.com/sivaprasad9/githubaug04.git'
	}
	stage('compile-package'){
		 withMaven({
		 bat "mvn clean install"
		 })
	}
	
}

