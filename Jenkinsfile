pipline{
		agent {
			label {
					label'built-in'
			customWorkspace "/project"
				}

			}
stages{
		stage("install-httpd"){
		
			steps {
		"yum install httpd -y"
		}	
			}
			
		stage("start-service"){
			steps {"service httpd start -y"
			}
			}
			
		stage("copy-paste"){
			steps {"/project/index.html /var/www/html"
			}
			}
			
 		}	

}
