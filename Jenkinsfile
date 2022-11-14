pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Bye') {
            when {
                branch 'main'
            }
            steps {
                echo 'Bye World'
            }
        }
    }
}
