pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
  agent any
   tools {
       gradle 'GRADLE'
   }
  stages {
    stage("build") {
      steps{
        echo 'building the application...'
         sh "./gradle assemble"
      }
    }
    stage("test") {
      steps{
        echo 'testing the application...'
         sh "./gradle test"
      }
    }
  }
}
