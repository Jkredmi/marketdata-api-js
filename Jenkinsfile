pipeline {
    agent {
    node {
	label 'built-in'
	customWorkspace '/home/ec2-user'
	}
	}
	stages {
	stage ('checkout') {
	steps {
	git clone https://github.com/Jkredmi/game-og-life.git
	cd game-of-life
	}
	}
	stage ('build') {
	steps {
		sh 'mvn clean install'
	}
	}
	stage ('Deploy') {
	steps {
		sh 'cp game-of-life/gameoglife-web/target/gameoflife-war/ /mnt/apache-tomcat-9.0.80/webapps'
	}
	}
	}
	}
	
