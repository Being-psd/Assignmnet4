pipeline {

agent {
			label{
				label 'built-in'
				customWorkspace "/mnt/myproject"
			}
}

stages{
			stage ('deploy'){
			steps{
			sh "sudo yum install httpd -y "
             
			}
		}
		stage ('start'){
				steps{
					
				sh "cp /mnt/myproject/index.html /var/www/html/"
					sh "chmod 777 /var/www/html/index.html"
					sh "systemctl start httpd"
            
				}
			}
}
}
