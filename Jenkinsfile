pipeline {
    agent none
    options {
        buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '3', daysToKeepStr: '90', numToKeepStr: '30')
    }
    stages {
        stage('Release') {
            steps {
                scm {
                    git('https://github.com/berzima1/Robot_academy.git')
                    credentials('github-ci-key')
                    }
                }
            }
        }
        stage('Deploy') {
            when { branch 'master' }
            steps {
                script {
                    echo "Running test suites..."
                    }
                }
        }
    }