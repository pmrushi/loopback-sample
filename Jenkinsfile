node {
    env.NODEJS_HOME = "${tool 'NodeJS 14.17.0'}"
    env.PATH="${env.NODEJS_HOME}/bin:${env.PATH}"
    sh "node -v"
    sh "npm -v"

	stage('Git Clone') {
		git 'https://github.com/pmrushi/loopback-sample.git'
	}
	stage('Build') {
		sh 'npm i'
	}
	stage('Test') {
		sh 'npm run test'
	}
}
