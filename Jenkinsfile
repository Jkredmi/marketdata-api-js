pipeline {
    agent {
    node {
	label 'built-in'
	customeWorkspace '/home/ec2-user'
	}
	}
	parameters {
	string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'who should i say hello to?')
	}
	stages {
	stage ('checkout') {
	steps {
	echo "Hello ${params.PERSON}"
	}
	}
	stage ('build') {
	steps {
	echo "Hello ${params.PERSON}"
	}
	}
	stage ('Deploy') {
	steps {
	echo " Hello ${params.PERSON}"
	}
	}
	}
	}
	
