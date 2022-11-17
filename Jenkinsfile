pipeline {

    agent any
    /*triggers {
      #triggered by changes in every branch
    }*/
    stages {
      stage ('first-stage'){
        when { env.GIT_BRANCH 'main' }
        steps{
          echo 'hello world'
        }
      }
      stage('second-stage'){
        when {
          not {
            env.GIT_BRANCH'main'
          }
          not {
            env.GIT_BRANCH'Ehsan'
          }
        }
        steps{
            echo "${env.GIT_BRANCH}"
        }
      }

    }
}
