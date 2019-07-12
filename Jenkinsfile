pipeline{
	agent any
	stages{
		stage("hello"){
			steps{
				sh 'echo "ansible test2"'
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