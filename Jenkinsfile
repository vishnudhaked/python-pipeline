pipeline {
	agent any
	stages {
		stage ("pull scm python test") {
			steps {
				git branch: 'python', url: 'https://github.com/wssrronak/python-pipeline.git'
				}
			}
		stage ("Build") {
			steps {
				sh 'python3 -V'
				sh 'python3 cp.py'
				}
			}
		stage ("Test") {
			steps {
				sh 'python3 test.py'
				}
			}
		}
	}
