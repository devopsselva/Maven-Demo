pipeline{
    agent any
   stages{
       stage ("git"){
           steps {
               git 'https://github.com/devopsselva/Maven-Demo.git'
           }
       }
       stage ("installation"){
           steps {
               bat 'mvn install'
           }
       }
       stage ("deploy"){
          steps {bat '''xcopy /y "C:\\Program Files (x86)\\Jenkins\\workspace\\pipe declare\\multi-module\\webapp\\target\\webapp.war" "C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps"
'''
}
     }
 }
}
