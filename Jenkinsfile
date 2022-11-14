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
                branch 'Main'
            }
            steps {
                echo 'Bye World'
            }
        }
    }
}
