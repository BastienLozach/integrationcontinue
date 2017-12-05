pipeline {
	agent any
	stages {
	    stage('Sonar'){
    			steps {
    				sh 'mvn sonar:sonar'
    			}
    		}
		stage('Build'){
			steps {
				sh 'mvn -B -DskipTests clean package'
				sh 'mvn test'
				sh 'ls target'
			}
		}
	}
}