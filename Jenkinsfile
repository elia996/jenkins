pipeline{
	agent any
	stages{
		stage("ansible"){
			steps{
				sh 'echo "ansible test"'
			}
		}
		stage("test"){
			steps{
				ansiblePlaybook playbook: 'myplaybook.yml'
			}
		}
	}
}