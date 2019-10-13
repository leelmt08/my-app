node {
   stage('SCM Checkout'){
	git  'https://github.com/leelmt08/my-app/'
   }

	stage ('Compile package'){
	//Get mvn home path
	def mvnHome = tool name: 'maven_3_6_2', type: 'maven'
		bat "${mvnHome}/bin/mvn package"
	}
	
	         stage('testing stage') {
             steps {
		def mvnHome = tool name: 'maven_3_6_2', type: 'maven'
                bat "${mvnHome}/bin/mvn test"
        }
		 }
}
	
