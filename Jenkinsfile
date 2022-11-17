pipeline {

    agent any
    /*triggers {
      #triggered by changes in every branch
    }*/
    stages {
      stage ('first-stage'){
        when { env.GIT_BRANCH in "orogin/main" }
        steps{
          echo 'hello world'
        }
      }
      stage('second-stage'){
        when {
          not {
            env.GIT_BRANCH in "main"
          }
          not {
            env.GIT_BRANCH in "Ehsan"
          }
        }
        steps{
            echo "${env.GIT_BRANCH}"
        }
      }

    }
}
