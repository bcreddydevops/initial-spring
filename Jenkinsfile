pipeline {
    agent any
    tools{
        maven 'maven-3'
    }

    stages {
        stage('git checkout') {
            steps {
                 git url:'https://github.com/bcreddydevops/initial-spring.git', branch: 'master'
                 sh 'ls -l'
                 sh 'pwd'
            }
        }
        stage('maven build') {
            steps{
                sh 'mvn clean install'
            }
        }
    }
}
