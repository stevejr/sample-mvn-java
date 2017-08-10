pipeline {
    agent {
        docker {
            label 'swarm'
            image 'maven:3.5-jdk-7-alpine'
        }
    }
        
    stages {
        stage('Build') {
            steps {
                sh "cd NumberGenerator && mvn package"
            }
        }
    }
}

