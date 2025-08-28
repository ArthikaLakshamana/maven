pipeline {
    agent any

    stages {
        stage('Compile') {
            steps {
                echo 'Hello compile stage'
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Hello Test stage'
                sh 'mvn test'
            }  
        }
        stage('package') {
            steps {
                echo 'Hello package stage'
                sh 'mvn package'
            }  
        }    
      stage('deploy') {
            steps {
                echo 'Hello deploy stage'
                sh ' java -cp target/my-app-1.0-SNAPSHOT.jar com.mycompany.app.App'
            }  
        }    
    }
}
