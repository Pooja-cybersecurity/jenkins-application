pipeline {
  agent any 
  stages {
  stage('Compiled stage') {
  
  steps {
  withMaven(maven: 'Maven')
  { echo "mvn clean compiled Stages"}
  } 
 }
 
 stage('Testing stage') {
  
  steps {
  withMaven(maven: 'Maven')
  { echo "mvn clean Testing Stages"}
  } 
 }
 
 stage('Deployment stage') {
  
  steps {
  withMaven(maven: 'Maven')
  { echo "mvn clean Deployment Stages"}
  } 
 }
 
 
  }



}
