pipeline {
	agent any
	stages {
		stage('Build'){
			steps {
				sh 'mvn -B -DskipTests clean package'
				sh 'mvn test'
				sh 'ls target'
			}
		}
	}
}