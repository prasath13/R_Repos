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
                                            not { branch "master" }
                                  }
                                  steps { echo "Hello" }
                            }
                             stage ('four'){
                                  parallel {
                                            stage ('unit test') { 
                                                      steps { echo "running the unit test..." }
                                            }
                                            stage ('Integration test') {
                                                      agent {
                                                            steps { echo "running the integration test..." }
                                                      }
                                                   
                                            }
                                  }
                             }
                  }
}
