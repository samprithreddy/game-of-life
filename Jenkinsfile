pipeline {
    agent {label 'jdk_8'}
    stages {
        stage('vcs') {
            steps {
                git url: 'https://github.com/samprithreddy/game-of-life.git',
                     branch: 'declarative'
            
            }
        } 
        stage('package') {
            steps {
                 sh """
                      export PATH=/usr/lib/jvm/java-8-openjdk-amd64/bin:$PATH
                      mvn package
                    """  
                    }
        }
    }
}
