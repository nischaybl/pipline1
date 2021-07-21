pipeline {
	agent any 
	stages {
		stage('BUILD') {
			steps {
				sh '''
					pwd
					echo This is the fist stage: BUILD
				'''
			}	
		}
		
		stage('TEST') {
			steps {
				sh '''
					echo This is the fist stage: TEST
				'''
			}	
		}
		
		stage('DEPLOY') {
			steps {
				sh '''
					pwd
					echo This is the fist stage: DEPLOY
				'''
			}	
		}
	}
}
