node('Docker01') {
    stage('Checkout') {
            echo 'Checkout'
            sh '''echo Checkout steps'''
	    sh '''rm -rf packerpipeline'''
	    sh '''git clone https://github.com/wagnermh/packerpipeline.git'''
    }
    stage('Initial') {
            echo 'Initializing'
	    sh '''cd packerpipeline && ls -lh && packer init .'''
    }
    stage('Format') {
            echo 'Formating'
	    sh '''pwd && packer fmt . &&  ls -lh'''
    }
    stage('Validate') {
            echo 'Validating'
	    sh '''pwd &&  ls -lh && packer validate .'''
    }
	stage('Build') {
            echo 'Building'
    }
}
