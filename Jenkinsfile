pipeline{
	agent any
	stages{
		stage("test"){
			steps{
				ansiblePlaybook inventory: 'hosts.txt', playbook: 'myplaybook.yml'
			}
		}
	}
}