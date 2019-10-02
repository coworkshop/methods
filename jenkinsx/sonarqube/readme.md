# sonarqube
This procedure was borrowed from https://github.com/jenkins-x/jx/issues/536

Sonarqube can be installed in an existing JenkinsX installation using the following commands.
Modify the sonarqube-ingress.yml with your domain name, and if you need other plugins pre-installed, in sonarqube.yml


	jx step helm install --set-file sonarqube.yml --name dev stable/sonarqube --namespace jx

	kubectl apply -f sonarqube-ingress.yml  
	
	
Adding sonarqube processing as part of a build pipeline can be done as in the [jenkins-x.yml](jenkins-x.yml) file

