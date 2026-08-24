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
	
	stage('Validation') {
	    steps {
		echo 'Running code validation checks...'
          	sh 'echo "Validating file structure..."'
		sh 'ls -la'
            }
	}

	stage('Test') {
	    steps {
		echo 'Running tests...'
		sh 'echo "All tests passed"'
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
