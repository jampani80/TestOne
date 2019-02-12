pipeline {
 agent any
 stages {
 
  stage('SetUp') {
   steps {
    
    
    sh "java -version"
     sh "ant -d -version"
    
    }
  }
  
  stage('Build') {
 steps {
   sh "'ant build.xml'"
 }
 }
 stage('Run') {
 steps {
 sh 'echo srini'
 }
 }
 }
}
