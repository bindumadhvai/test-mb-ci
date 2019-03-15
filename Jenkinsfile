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
      }
      if (env.BRANCH_NAME == 'dev') {
             echo 'run this stage - ony if the branch = dev branch'
      }
      if (env.BRANCH_NAME == 'test'){
             echo 'run this stage - ony if the branch = test branch'
      }
      if(env.BRANCH_NAME !== /(dev|master|test)/) {
       echo "this is feature barcnh" 
      }
  }  
}
