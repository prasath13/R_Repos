pipeline {
          agent any
                   stages {
                            stage ('one'){
                                  steps { echo 'Hi, this is Prasath from cts' }
                            }
                            stage ('two'){
                                  steps { input ('Do you want to proceed?') }
                            }
                            stage ('iii'){
                                  when {
                                        not { 
                                                  branch "master"
                                                  echo "master"
                                        }
                                  }
                                  steps { echo "Hello" }
                            }
                  }
}
