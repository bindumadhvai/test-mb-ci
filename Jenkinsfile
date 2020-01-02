pipeline {
    options {
        quietPeriod 1200
        buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '', numToKeepStr: '3')
    }
    agent any
    stages {
        stage('3') {
            steps {
                println("Hello")
            }
        }
    }
}
