pipeline {
  agent any 
  stages {
   
  stage('Compiled stage') {
  
  steps {
    def @mvnHome = tool name: 'Maven', type: 'maven'
    withMaven(maven: 'Maven')
     {
       
        sh 'mvn clean compiled Stages'
      }
  } 
 }
 
 stage('Testing stage') {
  def mvnHome = tool name: 'Maven', type: 'maven'
  steps {
  withMaven(maven:'Maven')
  { echo "mvn clean Testing Stages"}
  } 
 }
 
 stage('Deployment stage') {
  def mvnHome tool = name: 'Maven', type: 'maven'
  steps {
  withMaven(maven:'Maven')
  { echo "mvn clean Deployment Stages"}
  } 
 }
 
 
  }



}
