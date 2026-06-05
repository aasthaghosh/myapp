pipeline {
agent any

stages {

    stage('Build') {
        steps {
            bat 'docker build -t myapp .'
        }
    }

    stage('Deploy') {
        steps {
            bat 'docker rm -f myapp-container 2>nul'
            bat 'docker run -d --name myapp-container -p 3000:3000 myapp'
        }
    }

}

}
