pipeline {

	agent {

				label {

						label "built-in"
						customWorkspace "/mnt/vel-app-1"
				}	
	}

	stages {

			stage ("install httpd") {

					steps {

							sh "yum install httpd -y"
						}
			}

		stage ("start httpd") {

					steps {

							sh "service httpd start"
						}
			}

		stage ("deploy index") {

					steps {

							sh "cp -r index.html /var/www/html/"
							sh "chmod -R 777 /var/www/html/index.html"
						}
			}
		
		}

}
