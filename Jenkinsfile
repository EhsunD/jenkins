pipeline {
    agent any

    stages {
 stages {
        stage('Hello') {
            when {
                branch 'main'
            }
            steps {
                script{
                    if (env.BRANCH_NAME == 'main') {
                        echo 'we are main branch'
                    }
                }
                echo 'Hello World'
            }
        }
        stage('master') {
            steps {
                script{
                    if (env.BRANCH_NAME == 'master') {
                        echo 'we are master branch'
                    }
                }
            when {
                branch 'master'
            }
            steps{
                echo 'we are master'
            }
        }
    }
