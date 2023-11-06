pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                dir("Muskan_RestfulAndSoapWS") {
		bat "mvn clean"
	}
            }
        }
        stage('Compile') {
            steps {
	dir("Muskan_RestfulAndSoapWS") {
		bat "mvn compile"
	}
            }
        }
        stage('Test') {
            steps {
	dir("Muskan_RestfulAndSoapWS") {
		bat "mvn test"
	}
            }
        }
        stage('Result') {
            steps {
                echo "Result"
            }
        }
    }
}