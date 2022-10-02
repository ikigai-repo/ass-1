pipeline{
		agent {
			label {
					label'built-in'
			customWorkspace "/project"
				}

			}
stages{
		stage("install-httpd"){
		
			steps {
				sh"yum install httpd -y"
		}	
			}
			
		stage("start-service"){
			steps {
				sh"service httpd start -y"
			}
			}
			
		stage("copy-paste"){
			steps {
				sh"/project/index.html /var/www/html"
			}
			}
			
 		}	

}
