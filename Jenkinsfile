pipeline {
    agent {label 'jdk_8'}
    stages {
        stage(vcs) {
            steps {
                git url: 'https://github.com/samprithreddy/game-of-life.git',
                branch: 'declarative'
            
            }
        } 
        stage('package') {
            steps {
                sh 'maven package'
            }
        }
    }
}
