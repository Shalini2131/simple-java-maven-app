pipeline {
    agent any
	tools {
        maven "MAVEN"
        jdk "JDK"
    }
    stages {
        stage ('Compile Stage') {

            steps {
                    bat 'mvn clean install'
            }
        }

        stage ('Testing Stage') {

            steps {                
                    bat 'mvn test'
            }
        }


        stage ('Deployment Stage') {
            steps {
                    bat 'mvn deploy'
            }
        }
    }
}