pipeline{
    agent any
   stages{
       stage ("scm"){
           steps {git 'https://github.com/pandian3k/Maven-Demo.git' }
       }
       stage ("BUILD"){
           steps {bat label: '', script: 'mvn clean'
           bat label: '', script: 'mvn install' }
       }
       stage ("deploy"){
          steps {sh label: '', script: 'cp -rp "C:\\Program Files (x86)\\Jenkins\\workspace\\declare\\multi-module\\webapp\\target\\webapp.war"  "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"'}
       }
       
   }   
 }
