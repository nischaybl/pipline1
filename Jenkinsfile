pipeline {
	agent any  
	stages {
		stage('BUILD') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: BUILD
				'''
			}	
		
		stage('TEST') {
			parallel { 
				stage('TEST1') {
					agent { label 'docker-agent' }
					steps {
						sh 'sleep 5'	
						echo "TESTING PHASE1"
					}	

				}
				stage('TEST2') {
					agent { label 'agent1' }
					steps {
						sh 'sleep 5'	
						echo "TESTING PHASE2"
					}	

				}
				stage('TEST3') {
					agent { label 'master' }
					steps {
						sh 'sleep 5'	
						echo "TESTING PHASE3"
					}	
					
				}
				stage('TEST4') {
					steps {
						sh 'sleep 5'
						echo "TESTING PHASE4"
					}	
					
				}
			}	
				
		}
		
		stage('DEPLOY') {
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
}
