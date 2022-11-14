pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script{
                    if (env.BRANCH_NAME == 'main') {
                        echo 'we are main branch'
                    }
                }
            }
        }
        stage('master') {
            steps {
                script{
                    if (env.BRANCH_NAME == 'master') {
                        echo 'we are master branch'
                    }
                }
            }
        }
    }
}
