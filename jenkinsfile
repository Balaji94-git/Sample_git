pipeline {
    agent any

    stages {
        stage('Git Connect') {
            steps {
                git 'https://github.com/Balaji94-git/Sample_git.git'
                echo 'Git connection success..'
            }
        }
        stage('Build') {
            steps {
                 bat label: '', script: 'Build.bat'
            }
        }        
        stage('Test') {
            steps {
                bat label: '', script: 'Test.bat'
            }
        }
        stage('Deploy') {
            steps {
                bat label: '', script: 'Deploy.bat'
            }
        }
    }
}
