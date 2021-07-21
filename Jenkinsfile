pipeline {
	agent none
	stages {
		stage('BUILD') {
			agent 'slave'	
				steps {
					sh '''
						pwd
						echo This is the fist stage: BUILD
					'''
			}	
		}
		parallel {
		stage('TEST') {
			agent 'master'	
				steps ('TEST1') {
					sh '''
						echo This is the fist stage: TEST
	      		}		'''
				steps ('TEST2') {
					sh '''
						echo This is the fist stage: TEST
			}		'''
						
		}	
			
	}
		
		stage('DEPLOY') {
			agent 'slave'
				steps {
					sh '''
						pwd
						echo This is the fist stage: DEPLOY
					'''
				}	
			}
		}
	}
}
