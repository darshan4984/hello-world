node{
	stage('Checkout project from GIT') {
		echo 'Checking out project from GIT...'
		git url: 'https://github.com/darshan4984/hello-world.git'
	}
	stage('compile') {
		echo 'Compile the project..'
		def mvnHome = tool 'Maven 3.3.9'
		def mvnCMD = "${mvnHome}/bin/mvn"
		sh "${mvnCMD} clean package"
	}
}
