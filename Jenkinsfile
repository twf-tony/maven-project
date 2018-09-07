pipeline {
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'mvn clean package'
                sh -ex "docker build . -t tomcatwebapp:${env.BUILD_NUMBER}"
            }
        }
    }
}
