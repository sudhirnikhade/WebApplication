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
     echo "Hi, This is Deploy step"
     }
  }
}

}
