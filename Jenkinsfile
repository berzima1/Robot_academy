pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                bat 'c:\\Python27\\Scripts\\robot.exe ${env.WORKSPACE}\\Robot_academy.robot' 
            }
        }
    }
}