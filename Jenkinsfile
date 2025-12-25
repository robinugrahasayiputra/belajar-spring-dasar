pipeline {
    agent any
    stages {
        stage("Build"){
            steps {
                echo("Hello Mother fucker!")
            }
        }
        stage("test"){
            steps {
                echo("Hello Mother fucker!- 2")
            }
        }
        stage("Deploy"){
            steps {
                echo("Hello Mother fucker! - 3")
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