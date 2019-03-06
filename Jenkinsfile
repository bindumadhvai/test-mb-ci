node {
  stage ('hello') {
      echo "Hello"
  }
  stage('test') {
            when {
                branch 'master'
            }
            steps {
                echo "master" 
            }
        }
    stage('test') {
            when {
                branch 'dev'
            }
            steps {
                echo "dev" 
            }
        }
}
