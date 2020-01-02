pipeline {
    agent any
    options {
        quietPeriod 1200
        buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '3')
    }
    stages {
        stage('3') {
            steps {
                println("Hello")
            }
        }
    }
}
