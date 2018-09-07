pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'mvn clean package'
                sh "/usr/local/Cellar/docker/18.06.1/bin/docker build . -t tomcatwebapp:${env.BUILD_NUMBER}"
            }
        }
    }
}
