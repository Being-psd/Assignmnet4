pipeline {

agent {
			label{
				label 'built-in'
			}
}

stages{
			stage ('apache-run'){
			steps{
			sh "sudo yum install httpd -y "
                      sh "systemctl start httpd"
                      sh "cp -r index.html /var/www/html"
                      sh chmod -R 777 /var/www/html"
				}
			}
}
}

		
										
		
