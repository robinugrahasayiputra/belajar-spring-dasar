pipeline {
    agent any
    stages {
        stage("Hello"){
            steps {
                echo("Hello Mother fucker!")
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