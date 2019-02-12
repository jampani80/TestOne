pipeline {
 agent any
 stages {
 
 
  
  stage('Build') {
 steps {
  withAnt(installation: 'ant') {
   
   sh 'ant'
  }
  }
 }
 stage('Run') {
 steps {
 sh 'echo srini'
 }
 }
 }
}
