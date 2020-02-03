pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh 'c:\Python27\Scripts\robot.exe C:\Local_Robot_Framework\Robot_academy\Robot_academy.robot' 
            }
        }
    }
}