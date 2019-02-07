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
                sh  "git config --global user.name 'itachiuhia'"
                sh "git config --global user.email '06harshgtm@gmail.com'"
                sh "git init"
                sh "git checkout -b 'master'"
                sh 'git add Jenkinstest.class'
                sh "git commit -m 'Final commit'"
                sh "git push origin master"
            }
        }
    }
}
