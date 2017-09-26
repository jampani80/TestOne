pipeline {
 agent any
 stages {
 stage('build') {
 steps {
 sh 'ant build.xml'
 sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
 sh 'jar -cvmf MANIFEST.MF TestOne.jar *.class'
 }
 }
 }
}
