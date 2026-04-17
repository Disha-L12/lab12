pipeline{
  agent any
  tools{
     maven 'Maven'
     }
  stages{
    stage('Checkout'){
    steps{
        git branch:'master',url:'http://github.com/Disha-L12/lab12.git'
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
