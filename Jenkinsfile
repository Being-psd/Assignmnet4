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
			sh " sudo yum install httpd -y "
             
			}
		}
		stage ('start'){
				steps{
					sh "chmod -R 777 /mnt/myproject/index.html"
				sh "sudo cp -r /mnt/myproject/index.html /var/www/html/index.html"
					sh "sudo chmod -R 777 /var/www/html/index.html"
					sh "service httpd start"
            
				}
			}
}
}
