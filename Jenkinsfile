pipeline {
    agent any
    stages {
            stage('file creation') {
                steps {
                    sh """
                    mkdir /test2
                    """
            }
        }
		    stage('make directory') {
			    steps {
			        sh """
				    touch /opt/testfile2.txt
				    """
        }
    }
		    stage('hello directory') {
			    steps {
			        sh """
				    cp -Rp /opt/testfile2.txt /test1
				    """
			}
		}
    }
}
