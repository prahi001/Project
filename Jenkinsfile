pipeline{
	agent any
		stages {
			stage ('compile stage') {
				steps {
					withMaven(maven : 'M2_HOME') {
						sh 'mvn clean compile'
						}
					}
				}
	
			stage ('testing stage') {
				steps {
					withMaven(maven : 'M2_HOME') {
						sh 'mvn test'
						}
					}
				}
			stage ('deploy stage') {
				steps {
					withMaven(maven : 'M2_HOME') {
						sh 'mvn deploy'
						}
					}
				}
			}
		}
