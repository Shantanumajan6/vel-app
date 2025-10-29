pipeline {
		agent {
		
				label {
				
						label "built-in"
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
		
