@Library("shared") _
pipeline {
    agent any

    stages {
        stage('not hello'){
            steps {
                script {
                    hello()
                }
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
                sh ''' 
                cd meow
                echo "Hello World" > test.txt
                '''
            }
        }
    }
}
