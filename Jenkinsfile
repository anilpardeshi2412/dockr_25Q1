pipeline {
			agent {
					label {
								label "built-in"
								customWorkspace "/mnt/dock15"
							}
				}		
	stages {
		
		stage ('docker httpd') {
			
				steps {
			
				sh '''
						docker run -dp 150:80 --name c15 httpd
						docker cp /mnt/dock1/index.html c15:/usr/local/apache2/htdocs/								
					
					'''
					}			
				}	
					
			}		
}
