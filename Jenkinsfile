pipeline{
agent any
stages{
stage('Clone Repository'){steps{
git branch: 'main' ,
 url:'https://github.com/ankitjha100/mavenselenium.git' }
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
 stage('Execution'){
  steps{
   sh 'mvn exec:java -Dexec.mainClass="com.example.App"'
  }
 }
 }
  post {
 success {
 echo 'www.saucedemo.com'
 }
 failure {
 echo 'Build failed!'
 }
 }
}

