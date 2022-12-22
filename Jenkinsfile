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
			}
		}
		stage ('apache-run'){
				steps{
				sh "cp -r index.html /var/www/html"
            
				}
			}
}
}

		
										
		
