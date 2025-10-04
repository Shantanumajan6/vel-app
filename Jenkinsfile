pipeline {

		agent any
		
		stages {
		
				stage ('one') {
				
					steps {
					
								echo "hello world"
								sleep 10
					}
				}
				
			}
			
			post {
			    always {
			           echo "build done"   
					sleep 10
			    }
			    }   
					

}
