pipeline {
	agent none
	stages {
		stage('BUILD') {
			agent 'master'	
				steps {
					sh '''
						pwd
						echo This is the fist stage: BUILD
					'''
			}	
		}
		parallel {
		stage('TEST') {
			agent 'test'	
				steps ('TEST1') {
					sh '''
						echo This is the fist stage: TEST
	      		}		'''
				steps {'TEST2') {
					sh '''
						echo This is the fist stage: TEST
			}		'''
						
		}	
			
	}
		
		stage('DEPLOY') {
			agent 'master'
				steps {
					sh '''
						pwd
						echo This is the fist stage: DEPLOY
					'''
			}	
		}
	}
}
