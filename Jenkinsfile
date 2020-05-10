pipeline {
agent any
stages{
  stage ('Build') {
     steps {
     withMaven(maven : 'M3'){
     echo "Hi, This is compile step"
     sh 'mvn clean compile'
     }
     }
  }
   stage ('Test') {
     steps {
     withMaven(maven : 'M3'){
     echo "Hi, This is package step"
     sh 'mvn clean install'
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
