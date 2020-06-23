pipeline {
  agent any 
  stages {
    tool name: 'Maven', type: 'maven'
  stage('Compiled stage') {
  
  steps {
    withMaven(maven: 'Maven')
     {
        sh 'mvn clean compiled Stages'
      }
  } 
 }
 
 stage('Testing stage') {
  
  steps {
  withMaven(maven:'Maven')
  { echo "mvn clean Testing Stages"}
  } 
 }
 
 stage('Deployment stage') {
  
  steps {
  withMaven(maven:'Maven')
  { echo "mvn clean Deployment Stages"}
  } 
 }
 
 
  }



}
