pipeline {
	agent any
    stages {
        stage('Build') {
            steps {
			    echo 'Building..'
				checkout scm
				sh 'bun install'
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
				sh 'bun run build'
            }
        }
    }
}
