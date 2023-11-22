pipeline {
agent{
label{
		label "httpd"
		customWorkspace "/mnt/vel-app"
}
}

stages {

		stage ("httpd"){
			steps {
		              sh "yum install httpd -y"
                              sh "cp -r index.html /var/www/html"
                              sh "chmod -R 777 /var/www/html/"
			}
		
		}
		
		
		
		

}

}
