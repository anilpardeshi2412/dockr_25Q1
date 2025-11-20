pipeline {
			agent {
					label {
								label "built-in"
								customWorkspace "/mnt/dock12"
							}
				}		
	stages {
		
		stage ('docker httpd') {
			
				steps {
			
				sh '''
						docker run -dp 130:80 --name c13 httpd
						docker cp /mnt/dock1/index.html c13:/usr/local/apache2/htdocs								
					
					'''
					}			
				}	
					
			}		
}
