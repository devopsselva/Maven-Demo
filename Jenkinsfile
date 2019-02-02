pipeline {
 agent any
 stages {
     stage ('SCM'){
         steps {
             git 'https://github.com/devopsselva/Maven-Demo.git'
         }
     }
     stage ('BUILD'){
         steps {
             bat 'mvn clean'
             bat 'mvn install'
         }
     }
    stage ('DEPLOY'){
         steps {
                sh 'cp -rp "C:\\Program Files (x86)\\Jenkins\\workspace\\pipeline\\multi-module\\webapp\\target\\webapp.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'
         }
     }
 }
}
