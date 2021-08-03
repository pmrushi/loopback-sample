node {
	stage('Git') {
		git 'https://github.com/pmrushi/loopback-sample.git'
	}
	stage('Build') {
		sh 'npm i'
	}
	stage('Test') {
		sh 'npm run test'
	}
}
