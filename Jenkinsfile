pipeline {
agent any
stages{
  stage ('Build') {
     steps {
      echo "Hi, This is compile step"
     withMaven(maven : 'M3'){
     bat 'mvn clean compile'
     }
     }
  }
   stage ('Test') {
     steps {
       echo "Hi, This is package step"
     withMaven(maven : 'M3'){
          bat 'mvn clean install'
     }
     }
  }
   stage ('Deploy') {
     steps {
     echo "Hi, This is Deploy step"
     }
  }
}

}
