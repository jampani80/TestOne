pipeline {
 agent any
 stages {
 
 
  
  stage('Build') {
 steps {
   env.JAVA_HOME="${tool 'java-1.8.0-openjdk-1.8.0.191.b12-0.amzn2.x86_64'}"
    env.PATH="${env.JAVA_HOME}/bin:${env.PATH}" // set java home in jdk environment
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
