def execute = "false"
def et = "frst"+ env.BRANCH_NAME
node {
  stage ('hello') {
      git credentialsId: 'BitBucket', url: 'https://github.com/bindumadhvai/test-mb-ci.git'
      echo et
  }
  
  
 /*   stage ('bye') {
      echo "NO master"
  }*/
  
  stage ('test') {
      if (env.BRANCH_NAME == 'master'){
             echo 'echo s3://$et'
             $execute = "true"
             echo $execute
      }
      else if (env.BRANCH_NAME == 'dev') {
             echo 'echo s3://$et'
             echo 'run this stage - ony if the branch = dev branch'
             $execute = "true"
      }
      else if (env.BRANCH_NAME == 'test'){
             echo 'run this stage - ony if the branch = test branch'
             $execute = "false"
      } else {
             echo "this is feature barcnh"
             $execute = "false"
      }
  } 
  
  if ($execute == "true") {
     stage ('ex') {
         echo "i am executed"
     } 
    stage ('do') {
          echo "best"
    }
  }
  
}
