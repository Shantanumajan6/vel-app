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
			
					
					stage ('stop httpd') {
					
							steps {
										sh "service httpd stop"
										sleep 5
							}	
					
					}

				stage ("delete-old-htmls") {

						steps {

								sh "rm -rf /var/www/html/*"

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
