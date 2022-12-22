pipeline {

agent {
			label{
				label 'slave-1'
			}
}

stages{
			stage ('deploy'){
			steps{
				sh "rm -rf *"
			sh "sudo yum install httpd -y "
                      sh "systemctl start httpd"
			}
		}
		stage ('start'){
				steps{
				sh "cp -r index.html /var/www/html"
				sh "chmod -R 777 /var/www/hmtl/index.html"
					sh "chkconfig httpd on"
            
				}
			}
}
}
