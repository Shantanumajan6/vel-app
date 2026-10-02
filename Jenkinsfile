// jenkins file for my scm repo

// my jenkins file for deployment


pipeline {

			agent {
						label {
									
									label "built-in"
									customWorkspace "/mnt/projects"
						
						}
			}
			
			stages {
			
					stage ('install httpd') {
					
							steps {
										sh "yum install httpd -y"
							}	
					
					}
					
					stage ('start httpd') {
					
							steps {
										sh "service httpd start"
							}	
					
					}
					
					stage ('deploy htmls') {
					
							steps {
										sh "cp -r index.html /var/www/html"
										sh "cp -r dev.html /var/www/html"
										sh "chmod -R 777 /var/www/html"
							}	
					
					}
			}
}
