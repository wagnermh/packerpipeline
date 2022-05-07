pipeline {
    agent Docker01
    stages {
        stage('Checkout') {
            steps  {
				echo 'Checkout'
            }
        }
		stage('Initial') {
            steps  {
				echo 'Initial'
				packer init .
            }
        }
		stage('Format') {
            steps  {
				echo 'Format'
				packer fmt .
            }
        }
		stage('Validate') {
            steps  {
				echo 'Validate'
				packer validate .
            }
        }
		stage('Build') {
            steps  {
				echo 'Build'
				packer build docker-alpine.pkr.hcl
            }
        }
    }
}
