node{
	stage('GIT Checkout'){
		git 'https://github.com/prahi001/Project.git'
	}
		stage ('Compile-package') {
					def mvnHome =  tool name: 'M2_HOME', type: 'maven'
					sh "${mvnHome}/bin/mvn package"
						
					}
		stage ('Install') {
					def mvnHome1 =  tool name: 'M2_HOME', type: 'maven'
					sh "${mvnHome1}/bin/mvn install"
						
					}
				}
