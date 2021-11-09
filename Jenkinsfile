pipeline {
  
    
    stages {
     
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean install package' 
            },
            steps
      {
        def dockerHome = tool 'myDocker'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
        }
    }
}
