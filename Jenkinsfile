pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/dhiraj/Documents/DevopsSoftwaare/apache-maven-3.9.5/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/pipeline1.war /home/dhiraj/Documents/DevopsSoftwaare/apache-tomcat-9.0.82/webapps'
			}}	
}}
