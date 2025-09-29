pipeline {

	agent any


	stages {
	    stage('Checkout') {
		steps {
			git branch: 'main', url: 'https://github.com/Unicron-2028/dockerized-django-notes-application.git'
		}
	     }

	    stage('Build Docker Images') {
		steps {
			sh 'docker-compose -f docker-compose.yml build'
		}
	    }

	    stage('Deploy') {
		steps {
			sh '''
			docker-compose -f docker-compose.yml down
			docker-compose -f docker-compose.yml up -d
			'''
		}
	     }
	}


	post {
		success {
			echo 'Pipeline finished successfully!'
		}
		failure{
			echo 'Pipeline failed!'
		}
	}
}
 




