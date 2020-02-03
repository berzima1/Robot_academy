pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh 'c:\Python27\Scripts\robot.exe .\Robot_academy.robot' 
            }
        }
    }
}