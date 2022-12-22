pipeline {

agent {
			label{
				label 'slave-1'
			}
}

stages{
			stage ('apache-run'){
			steps{
			sh "sudo yum install httpd -y "
                      sh "service httpd start"
			}
		}
		stage ('apache-copy'){
				steps{
				sh "cp -r index.html /var/www/html"
				sh "chmod -R 777 /var/www/hmtl/index.html"
            
				}
			}
}
}
