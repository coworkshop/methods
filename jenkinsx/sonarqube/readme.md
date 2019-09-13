# sonarqube
installed with


	jx step helm install --set-file sonarqube.yml --name dev stable/sonarqube

	kubectl apply -f sonarqube-ingress.yml  