pipeline {
    agent any
    stages {
        stage("Build"){
            steps {
                echo("start build")
				sh("./mvnw clean compile test-compile")
				echo("finish build")
            }
        }
        stage("test"){
            steps {
                echo("Hello Test")
				sh("./mvnw test")
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
