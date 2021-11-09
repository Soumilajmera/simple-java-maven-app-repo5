pipeline {
  
    
    stages {
      stage('Initialize'){
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean install package' 
            }
        }
    }
}
