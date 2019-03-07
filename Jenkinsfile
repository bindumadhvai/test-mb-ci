node {
  stage ('hello') {
      echo "master"
  }
  
 /*   stage ('bye') {
      echo "NO master"
  }*/
  
  stage ('test') {
      def userInput = input message: 'enter OK for deployment', ok: 'Yes', parameters: [booleanParam(defaultValue: false, description: '', name: 'Deploy')]
      echo ("deploy: "+userInput)
  }  
}
