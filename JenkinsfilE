pipeline {
    agent any

    stages {
        stage('Clone from GIT') {
            steps {
                git 'https://github.com/sudhanshukumar-ai/SpringBoot-25Feb21.git'
                sh '''
                echo "=========cloning the SpringBoot-25Feb21============="
                ls
                '''
            }
        }
        stage('Build from Maven') {
            steps {
                withMaven(maven: 'example-maven-name') {
				sh '''
                echo "=========Building the SpringBoot-25Feb21 Project============="
                ls
                mvn clean install
                ls
                '''
                }
                
            }
        }        
    }
}

