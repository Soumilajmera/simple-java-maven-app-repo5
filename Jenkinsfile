pipeline {
    agent {
        docker {
            image 'maven:latest' 
            args '-u root' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean install package' 
            }
        }
    }
}
