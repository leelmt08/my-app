node {
   stage('SCM Checkout'){
	git  'https://github.com/leelmt08/my-app/'
   }

	stage ('Compile package'){
	sh 'mvn package'
	}
}
