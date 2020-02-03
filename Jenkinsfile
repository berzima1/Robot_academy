pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Do some tests') { 
            steps { 
                bat 'c:\\Python27\\Scripts\\robot.exe "%WORKSPACE%\\Robot_academy.robot"' 
            }
        }
    }
}