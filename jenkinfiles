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
						docker run -dp 80:80 --name s1 httpd
						docker cp /mnt/dock1/index.html s1:/usr/local/apache2/htdocs/								
					
					'''
					}			
				}	
					
			}		
}
