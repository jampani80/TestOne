pipeline {
 agent any
 stages {
 
  stage('SetUp') {
   steps {
    
    env.ANT_HOME="${tool 'ant}"
    env.PATH = "${env.ANT_HOME}/bin:${env.PATH}"
    sh "java -version"
    withAnt(installation: 'ant') {
    //  echo "Test ant"
      sh "ant -d -version"
    }
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
