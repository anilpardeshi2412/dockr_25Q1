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
						docker run -dp 90:80 --name c2 httpd
						docker cp /mnt/dock1/index.html c2:/usr/local/apache2/htdocs/								
					
					'''
					}			
				}	
					
			}		
}
