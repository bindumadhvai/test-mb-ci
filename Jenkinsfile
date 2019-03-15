node {
  stage ('hello') {
      echo $env.BRANCH_NAME
  }
  
 /*   stage ('bye') {
      echo "NO master"
  }*/
  
  stage ('test') {
      when{
             branch 'master'
      }
      steps {
             echo 'run this stage - ony if the branch = master branch'
      }
      when{
             branch 'dev'
      }
      steps {
             echo 'run this stage - ony if the branch = dev branch'
      }
      when{
             branch 'test'
      }
      steps {
             echo 'run this stage - ony if the branch = test branch'
      }
  }  
}
