pipeline {
agent{
label{
		label "httpd"
		customWorkspace "/mnt/directory"
}
}

stages {

		stage ("httpd"){
			steps {
		               sh "sudo yum install httpd -y"
			       sh "sudo service httpd start"
                               sh "sudo cp -r index.html /var/www/html"
                               sh "sudo chmod -R 777 /var/www/html/"
				sh "sudo service httpd restart"
				
			}
		
		}
		
		
		
		

}

}
