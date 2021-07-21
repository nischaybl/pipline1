pipeline {
	agent nano 
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
		
		stage('TEST') {
			agent 'test'	
				steps {
					sh '''
						echo This is the fist stage: TEST
					'''
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
