pipeline {
	agent nano 
	stages {
		stage('BUILD') {
			agent 'agent1'
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: BUILD
				'''
			}	
		}
		
		stage('TEST') {
			agent 'master'
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: TEST
				'''
			}	
		}
		
		stage('DEPLOY') {
			agent 'agent1'
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: DEPLOY
				'''
			}	
		}
	}
}
