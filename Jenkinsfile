pipeline {
			agent {
					label {
								label "built-in"
								customWorkspace "/mnt/dock13"
							}
				}		
	stages {
		
		stage ('docker httpd') {
			
				steps {
			
				sh '''
						docker run -dp 140:80 --name c14 httpd
						docker cp /mnt/dock1/index.html c14:/usr/local/apache2/htdocs								
					
					'''
					}			
				}	
					
			}		
}
