pipeline {
agent any

stages {

    stage('Build') {
        steps {
            bat 'docker build -t myapp .'
        }
    }

    stage('Run') {
        steps {
            bat 'docker run --rm myapp'
        }
    }

}

}

