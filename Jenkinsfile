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
                branch 'Ehsan'
            }
            steps {
                echo 'Bye World'
            }
        }
    }
}
