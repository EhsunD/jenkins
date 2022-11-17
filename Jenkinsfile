pipeline {

    agent any
    /*triggers {
      #triggered by changes in every branch
    }*/
    stages {
      stage ('first-stage'){
        when { Git_branch == 'main' }
        steps{
          echo 'hello world'
        }
      }
      stage('second-stage'){
        when {
          not {
            Git_branch =='main'
          }
          not {
            Git_branch =='Ehsan'
          }
        }
        steps{
          echo 'bye'
        }
      }

    }
}
