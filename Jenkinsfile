pipeline{
	agent any
	stages{
		stage("hello11"){
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
		stage("run shellscript"){
			steps{
				sh './test.sh'
			}
		}
	}
}