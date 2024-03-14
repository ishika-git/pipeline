pipeline {
   agent any 
   stages {
          stage('checkout') {
             steps {
                     chechout scm
                   }}
          stage('Build') {
             steps {
                     sh '/home/ishika/Documents/devops_software/apache-maven-3.9.6/bin/mvn install'
                   }}
          stage('deployment') {
             steps {
                     sh 'cp target/pipeline.war /home/ishika/Documents/devops_software/apache-tomcat-9.0.85/webapps'
                   }}
          }}
