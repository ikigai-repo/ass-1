pipeline{
		agent {
			label {
					label'slave-1'
			customWorkspace "/home/ec2-user"
				}

			}
stages{
		stage("install-httpd"){
		
			steps {
				sh"sudo yum install httpd -y"
		}	
			}
			
		stage("start-service"){
			steps {
				sh"sudo service httpd start"
			}
			}
			
		stage("copy-paste"){
			steps {
				sh"sudo cp /home/ec2-user/index.html /var/www/html"
			}
			}
			
 		}	

}
