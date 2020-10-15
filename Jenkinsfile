pipeline{
     agent any
        stages{
          stage(‘pull code from github’){
          steps{
            git credentialsId: 'github', url: 'https://github.com/pudugopi/firstJava.git'
          }
         }
       stage(‘Test’){
         steps{
          sh ‘make check’
         }
       }
       stage(‘Deploy’){
          steps{
            sh ‘make publish’
            }
        }
     }
}
