pipeline {
    agent any

    stages {
	stage('Checkout') {
           steps {
	       echo 'Checking out code from GitHub..'
	       checkout scm
	   }
	}
	
	stage('Build') {
	    steps {
		echo 'Building the application...'
		sh 'echo "Simulating build process..."'
	    }
	}

	stage('Test') {
	    steps {
		echo 'Running tests...'
		sh 'echo "Simulating test execution..."'
	    }
	}
    }


	post {
	    success {
		echo 'Pipeline completed successfully!'
	    }

	    failure {
		echo 'Pipeline failed. Check console ouput for details.'
	    }
	}
}
