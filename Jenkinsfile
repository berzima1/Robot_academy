pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                bat 'robot %WORKSPACE%\\Robot_academy.robot' 
            }
        }
    }
}