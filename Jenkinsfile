pipeline {
    agent any
    stages {
        stage("Build"){
            steps {
                echo("start build")
            }
        }
        stage("test"){
            steps {
                echo("Hello Test")
                script {
					def data = [
						"firstName" : "robb",
						"lastName" : "stark"
					]
					
					writeJSON(file:"data.json", json:data)
				}
            }
        }
        stage("Deploy"){
            steps {
                echo("Hello deploy")
            }
        }
    }
    
    post {
		always {
			echo ("after all this time? Always!")
		}
		success {
			echo ("success")
		}
		failure {
			echo ("failure")
		}
		cleanup {
			echo("cleanup")
		}
	}
}
