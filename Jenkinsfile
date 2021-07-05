pipeline {
    agent any
	tools {
        maven "MAVEN"
    }
    stages {
        stage ('Compile Stage') {

            steps {
                    bat 'mvn clean compile'
            }
        }

        stage ('Testing Stage') {

            steps {                
                    bat 'mvn test'
            }
        }
    }
}