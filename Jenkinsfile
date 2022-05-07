node('Docker01') {
    stage('Checkout') {
            echo 'Checkout'
            sh '''echo Checkout steps'''
	    sh '''git clone https://github.com/wagnermh/packer.git'''
    }
    stage('Initial') {
            echo 'Initializing'
    }
    stage('Format') {
            echo 'Formating'
    }
    stage('Validate') {
            echo 'Validating'
    }
	stage('Build') {
            echo 'Building'
    }
}
