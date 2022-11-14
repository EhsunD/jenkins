pipeline {

    agent any
    /*triggers {
      #triggered by changes in every branch
    }*/
    stages {
      stage('first-stage'){
        agent { branch 'main' }
        steps{
          echo 'hello world'
        }
      }
      stage('second-stage'){
        when {
          not {
            branch 'main'
          }
          not {
            branch 'Ehsan'
          }
        }
        steps{
          echo 'bye'
        }
      }

    }
}
