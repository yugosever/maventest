pipeline {
    agent any 
    stages {
        stage('Clean') { 
            steps {
                sh "mvn clean" 
            }
        }
        stage('Test') { 
            steps {
                sh "mvn test" 
            }
        }
        stage('Build') { 
            steps {
                sh "mvn package" 
            }
        }
         stage('Run') { 
            steps {
                sh "java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App" 
            }
        }
    }
}
