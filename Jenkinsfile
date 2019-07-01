pipeline {
  agent any
    stages {
      stage ('one'){
        steps {
          echo 'Hi, this is Prasath from cts'
        }
      }
      stage (2){
        steps {
          inputs('Do you want to proceed?')
        }
      }
      stage ('iii'){
        when {
          not {
            branch "master"
          }
        }
      }
    }
}
