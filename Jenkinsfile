pipeline {
	agent any
    stages {
        stage('Build') {
            steps {
			echo 'Building..'
		    	checkout scm
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
