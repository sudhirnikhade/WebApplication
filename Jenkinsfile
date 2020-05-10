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
       archive 'webapp/target/*.jar
       bat ''' copy webapp/target/*war G:\DEVOPS_FOLDER\DevOps-data\Week5\apache-tomcat-8.5.16\webapps'''
}

}
