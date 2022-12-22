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
                      sh "systemctl start httpd"
			}
		}
		stage ('apache-copy'){
				steps{
				sh "chown -R 777 /mnt/myproject/index.html"
				sh "cp /mnt/myproject/index.html /var/www/html"
				sh "chmod -R 777 /var/www/hmtl/index.html"
            
				}
			}
}
}

		
										
		
