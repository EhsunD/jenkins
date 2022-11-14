pipeline {
    agent any

    stages {
        stage('Hello') {
            when {
                branch 'main'
            }
            steps {
                echo 'Hello World'
            }
        }
        stage('Bye') {
            when {
                branch "Ehsan"
            }
            steps {
                echo 'Bye World'
            }
        }
    }
}
