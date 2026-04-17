pipeline{
  agent any
  tools{
     gradle 'Gradle'
    jdk "JDK'
     }
  stages{
    stage('Checkout'){
    steps{
        git branch:'master',url:'https://github.com/Disha-L12/lab12.git'
        }
        }
   stage('Build'){
   steps{
      sh 'gradle build'
      }
      }
   stage('Test'){
   steps{
      sh 'gradle test'
      }
      }
   stage('Run application'){
   steps{
     sh 'gradle run'
     }
     }
  post {
     success{
      echo "build successfully"
      }
      
     failure{
       echo "build fail"
       }
       }
       }
       }
