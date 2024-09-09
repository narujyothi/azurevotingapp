pipeline {
    agent { label 'ansible' }
    stages {
        stage('Clean Workspace') {
            steps {
                deleteDir() // Deletes the contents of the workspace
            }
        }
        stage('Clone Repository') {
            steps {
               
                git url: 'git@github.com:chumaedeogu/example-voting-app.git', branch: 'master'
            }
        }
    }
}
