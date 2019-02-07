pipeline {
    agent any
    stages {

        stage('run_testing'){
            steps {

                sh "javac Jenkinstest.java"
              }
        }

        stage('Deploy') {
            steps {
                sh "git init"
                sh 'git add Jenkinstest.class'
                sh "git commit -m 'Final commit'"
                sh "git push origin master"
            }
        }
    }
}
