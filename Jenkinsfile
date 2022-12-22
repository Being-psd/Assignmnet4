pipeline {

agent {
			label{
				label 'slave-2'
				customWorkspace "/mnt/myproject"			}
}

stages{
			stage ('apache-run'){
			steps{
			sh "sudo yum install httpd -y "
			}
		}
		stage ('apache-copy'){
				steps{
				sh "sudo cp /mnt/myproject/index.html /var/www/html"
				sh "sudo chmod -R 777 /var/www/hmtl/index.html"
					sh "sudo service httpd start"
            
				}
			}
}
}

		
										
		
