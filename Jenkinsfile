pipeline {
    agent Docker01
    stages {
        stage('Checkout') {
            steps  {
				echo 'Checkout'
				git clone https://github.com/wagnermh/packer.git
				cd  packer
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
