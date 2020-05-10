pipeline {
agent any
  tools{
  maven "M3" 
  }
stages{
  stage ('Build') {
     steps {
      echo "Hi, This is compile step"
          bat 'mvn clean compile'
       }
  }
   stage ('Test') {
     steps {
       echo "Hi, This is package step"
       bat 'mvn clean install'
     
     }
  }
   stage ('Deploy') {
     steps {
       archive 'webapp/target/*.war
       bat ''' copy C:\\Users\\Sudhir Nikhade\\.jenkins\\workspace\\Demo_Jenkinsfile\\webapp\target\\webapp.war G:\\DEVOPS_FOLDER\\DevOps-data\\Week5\\apache-tomcat-8.5.16\\webapps\\'''
}

}
