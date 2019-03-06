node {
  stage ('hello') {
      echo "Hello"
  }
  stage('test') {
            when {
                branch 'master'
            }
            steps {
                echo "bye" 
            }
        }
}
