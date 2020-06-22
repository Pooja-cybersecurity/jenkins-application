pipeline {
  agent any 
  stages {
  stage('Compiled stage') {
  
  steps {
  withMaven(maven: 'Maven')
  {}
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
