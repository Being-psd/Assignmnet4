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
			sh " yum install httpd -y "
             
			}
		}
		stage ('start'){
				steps{
					
				sh "cp /mnt/myproject/index.html /var/www/html/index.html"
					sh "chmod -R 777 /var/www/html/index.html"
					sh "service httpd start"
            
				}
			}
}
}
