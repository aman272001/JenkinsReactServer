pipeline {
	agent any
    stages {
        stage('git') {
            steps {
				git 'https://github.com/aman272001/JenkinsReactServer.git'
            }
        }
       stage('Build') {
            steps {
			    echo 'Building..'
				sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
				sh 'npm run build'
            }
        }
    }
}
