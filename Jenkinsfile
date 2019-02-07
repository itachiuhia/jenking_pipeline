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
                sh 'git add Jenkinstest.class'
                sh "git commit -m 'Final commit'"
                sh "git remote add origin https://github.com/itachiuhia/jenking_pipeline.git"
                sh "git push -u origin master"
            }
        }
    }
}
