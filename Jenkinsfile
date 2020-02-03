multibranchPipelineJob('RobotAcademy') {
    scm {
        git('https://github.com/berzima1/Robot_academy.git')
        credentials('github-ci-key')
    }
    triggers {
        scm('H/15 * * * *')
    }
    steps {
        script {
            echo "Running test suites..."
        }
    }
}