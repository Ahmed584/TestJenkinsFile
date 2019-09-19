pipeline {
    agent any
    stages {
        stage('clone'){
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/Ahmed584/TestJenkinsFile.git"
            }
        }
        stage('build'){
            steps {
                sh'''cd JenkinsTest/src/helloWorld/
                 javac Main.java'''
            }
        }
        stage('run'){
            steps {
                sh "cd JenkinsTest/src/ && java helloWorld/Main"
            }
        }
    }
}