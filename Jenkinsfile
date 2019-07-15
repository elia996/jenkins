pipeline{
	agent any
	stages{
		stage("hello11"){
			steps{
				script{
					def rootDir = pwd()
					def example = load "${rootDir}@script/common.groovy "
					example.printmsg("test")
				}
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