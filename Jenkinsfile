pipeline {

    agent any
    /*triggers {
      #triggered by changes in every branch
    }*/
    stages {
      stage ('first-stage'){
          steps{
              script{
          if ( env.GIT_BRANCH == "origin/main" ){
                  echo 'hello world'
        }
              }
          }
      }
      stage('second-stage'){
        when {
          not {
            branch "main"
          }
          not {
            branch "Ehsan"
          }
        }
        steps{
            echo "${env.GIT_BRANCH}"
        }
      }

    }
}
