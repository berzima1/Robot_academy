pipeline {
    agent none
    stages {
        stage('Get_code') {
            steps {
                scm {
                    git('https://github.com/berzima1/Robot_academy.git')
                    credentials('Git_cred')
                    }
                }
            }
        }
    }