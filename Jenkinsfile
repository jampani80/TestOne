pipeline {
 agent any
 stages {
 
  stage('SetUp') {
    env.JAVA_HOME="${tool 'jdk_8u181'}"
    env.ANT_HOME="${tool 'ant_1_10_5'}"
    env.PATH = "${env.JAVA_HOME}/bin:${env.ANT_HOME}/bin:${env.PATH}"
    sh "java -version"
    withAnt(installation: 'ant_1_10_5', jdk: 'jdk_8u181') {
    //  echo "Test ant"
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
