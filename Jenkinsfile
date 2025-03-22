@Library("shared") _
pipeline {
    agent {label 'slave'}

    stages {
        stage('jenkins sharing'){
            steps {
                script {
                    hello()
                }
            }
        }
        stage('Hello build folder') {
            steps {
                echo 'Hello testing'
                sh ''' 
                cd peacock 
                echo "Hello Worllld" > test.txt
                '''
            }
        }
    }
}
