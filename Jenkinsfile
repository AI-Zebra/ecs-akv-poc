pipeline {
  agent any
  environment {
    SECRET_KEY = credentials('secret-key')
  }
  stages {
    stage('Foo') {
      steps {
        echo SECRET_KEY
        echo SECRET_KEY.substring(0, SECRET_KEY.size() -1) // shows the right secret was loaded, don't do this for real secrets unless you're debugging 
      }
    }
  }
}
