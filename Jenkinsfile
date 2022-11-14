pipeline {

    triggers {
      # triggered by changes in every branch
    }
    stages {
      stage('first-stage'){
        when { anyOf { branch 'feature-branch/*'; branch 'main' } }
        steps{
          echo 'hello world'
        }
      }
      stage('second-stage'){
        when {
          not {
            branch 'release/*'
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
