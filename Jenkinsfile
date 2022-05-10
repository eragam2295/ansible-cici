pipeline {
    agent any
     tools {
         jdk  'openjdk 1.8'
         git  'Default'
         maven 'maven'
         dockerTool 'docker'
     }
     
    stages {
        stage ('scm checkout') {
            steps{
               git url:'https://github.com/eragam2295/simple-app.git'
        }
    }

       stage('mvn package'){
           steps{ 
             sh 'mvn clean package'
             sh 'pwd'
}
}
    }
