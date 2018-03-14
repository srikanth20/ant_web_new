#! groovy
node{
 stage('Source'){
     git 'https://github.com/srikanth20/ant_web_new.git'
 }
 
 stage('Build'){
    
    sh "ant -f build-mt.xml" 
 }
 stage('Send Email'){
     mail bcc: 'sgsrikanth482@gmail.com', body: 'Buils is done', cc: '', from: '', replyTo: '', subject: 'Build Status', to: 'devopstrainingblr@gmail.com'
 }
 /*stage('Archive'){
  archiveArtifacts '/Users/bhaskarreddyl/.jenkins/workspace/Pipeline-Project-Ant-Web/dist/SampleAntProject.war'
 }*/
}
