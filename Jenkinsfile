pipeline{
	agent any
	stages{
		stage("test"){
			steps{
				ansiblePlaybook playbook: 'myplaybook.yml'
			}
		}
	}
}