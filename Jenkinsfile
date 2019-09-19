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
                sh'''cd TestJenkinsFile/src/Main/
                 javac Main.java'''
            }
        }
        stage('run'){
            steps {
                sh "cd TestJenkinsFile/src/ && java helloWorld/Main"
            }
        }
    }
}
