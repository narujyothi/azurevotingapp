pipeline {
    agent { label '!ansible' }
    stages {
        stage('Clean Workspace') {
            steps {
                deleteDir() // Deletes the contents of the workspace
            }
        }
        stage('Clone Repository') {
            steps {
               
                git url: 'https://github.com/chumaedeogu/example-voting-app.git', branch: 'main'
            }
        }
    }
}
