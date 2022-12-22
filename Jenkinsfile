pipeline {

agent {
			label{
				label 'slave-1'
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
				sh "cp /mnt/myproject/index.html /var/www/html"
				sh "chmod -R 777 /var/www/hmtl/index.html"
					sh "systemctl start httpd"
            
				}
			}
}
}
