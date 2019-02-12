pipeline {
 agent any
 stages {
 
 
  
  stage('Build') {
 steps {
  withAnt(installation: 'ant') {
   
   sh 'ant TestOne/build.xml'
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
