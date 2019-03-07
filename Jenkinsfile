node {
  stage ('hello') {
      echo "master"
  }
  stage ('test') {
      def userInput = input message: 'enter OK for deployment', ok: 'OK', parameters: [booleanParam(defaultValue: false, description: 'Cancel', name: 'Deploy')]
      echo ("deploy: "+userInput)
  }  
}
