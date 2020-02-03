pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Do some tests') { 
            steps { 
                bat 'c:\\Python27\\Scripts\\robot.exe -d /results "%WORKSPACE%\\Robot_academy.robot"' 
            }
        }
        stage('Publish') {
            steps {
                script {
                    echo "Collecting artifacts..."
                    robotPublish()
                    echo "Reports published"
                }
            }
        }
    }
}
def robotPublish() {
    step([
        $class : 'RobotPublisher',
        outputPath : './results',
        outputFileName : "output.xml",
        reportFileName : 'report.html',
        logFileName : 'log.html',
        disableArchiveOutput : false,
        passThreshold : 100,
        unstableThreshold: 95.0,
        otherFiles : "*.png",
    ])
}