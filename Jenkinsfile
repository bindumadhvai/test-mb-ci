def execute = "false"
node {
  stage ('hello') {
      echo env.BRANCH_NAME
  }
  
 /*   stage ('bye') {
      echo "NO master"
  }*/
  
  stage ('test') {
      if (env.BRANCH_NAME == 'master'){
             echo 'run this stage - ony if the branch = master branch'
             $execute = "true"
             echo $execute
      }
      else if (env.BRANCH_NAME == 'dev') {
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
