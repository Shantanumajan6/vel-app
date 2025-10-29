pipeline {
		agent {
		
				label {
				
						label "slave-1"
						customWorkspace "/mnt/pipeline"
				}
		}
		
		
		stages {
		
				stage ("one") {
						steps {		
									sh "rm -rf *"
									sh "mkdir velocity"
						}
				}
		}
		
		post {
		    
		    always {
		            echo "thank you, job worked fine"   
		    }
		    }
		       
		}
		
