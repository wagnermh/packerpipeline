node('Docker01') {
    stage('Checkout') {
            echo 'Checkout'
            sh '''echo Checkout steps'''
	    sh '''git clone https://github.com/wagnermh/packerpipeline.git'''
    }
    stage('Initial') {
            echo 'Initializing'
	    sh '''cd packerpipeline'''
	    sh '''packer init .'''
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
