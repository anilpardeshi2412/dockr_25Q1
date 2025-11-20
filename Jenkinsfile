pipeline {
			agent {
					label {
								label "built-in"
								customWorkspace "/mnt/dock1"
							}
				}		
	stages {
		
		stage ('docker httpd') {
			
				steps {
			
				sh '''
						docker run -dp 120:80 --name c12 httpd
						docker cp /mnt/dock1/index.html c2:/usr/local/apache2/htdocs/								
					
					'''
					}			
				}	
					
			}		
}
