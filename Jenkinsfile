def execute = "false"
def text1 = "/var/lib/jenkins"
node {
  stage ('hello') {
      echo env.BRANCH_NAME
      text1 = "/var/lib"
  }
  
 /*   stage ('bye') {
      echo "NO master"
  }*/
  
  stage ('test') {
      if (env.BRANCH_NAME == 'master'){
        $text = "${text1}"
        sh script : ''' ls -al ${text1} '''
             execute = "true"
      }
      else if (env.BRANCH_NAME == 'dev') {
             echo 'run this stage - ony if the branch = dev branch'
      }
      else if (env.BRANCH_NAME == 'test'){
             echo 'run this stage - ony if the branch = test branch'
      } else {
             echo "this is feature barcnh" 
      }
  } 
  
  stage ('ex') {
    if (execute == "true") {
         echo "i am executed"
    }
  }
}
