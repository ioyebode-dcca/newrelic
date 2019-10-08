pipeline {
   agent any
   stages {
      stage ('one') {
                   steps {
                              echo 'Hi, this is for testing'
                              }
                 }
                 stage ('two') {
                   steps {
                                                            input('Do you want to proceed?')
                              }
                 }
                 stage ('three') {
                   when {
                                             not{
                                                            branch "master"
                                             }
                              }
                              steps {
                                             echo 'successful'
                              }
                 }
                 stage ('four') {
                  echo 'testing completed, thank you'
                 }
                 stage ('five') {
                                             paralle {
                                                            stage ('unit test') {
                                                                           echo 'testing codes againts test cases'
                                                            }
                                                            stage ('selenium tesing') {
                                                                           echo 'performing selenium testing for devsecOps'
                                                            }
                                             }
                 }
   }
}
