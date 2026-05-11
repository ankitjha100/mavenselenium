pipeline{
agent any
stages{
stage('Clone Repository'){
git branch:main ,url:'https://github.com/ankitjha100/mavenselenium.git' 
 }
 stage('Build') {
 steps {
 sh 'mvn clean compile'
 }
 }
 stage('Test Automation') {
 steps {
 sh 'mvn test'
 }
 }
 }
}

