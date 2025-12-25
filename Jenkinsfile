pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                if (isUnix()) {
                    sh 'mvn -B -DskipTests clean package'
                } else {
                    bat 'mvn -B -DskipTests clean package'
                }
            }
        }
    }
}