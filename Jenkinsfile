pipeline{
	agent any
	stages{
		stage("ansible"){
			steps{
				sh 'echo "ansible test1"'
			}
		}
		stage("ansible"){
			steps{
				sh 'echo "ansible test2"'
			}
		}
		stage("test"){
			steps{
				ansiblePlaybook playbook: 'myplaybook.yml'
			}
		}
	}
}