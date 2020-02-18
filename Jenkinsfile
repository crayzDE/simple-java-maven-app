pipeline {
    agent {
        docker {
            image 'maven:3-alpine' 
            args '-u docker'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
