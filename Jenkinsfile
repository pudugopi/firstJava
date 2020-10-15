Pipeline{
     Agent any
        Stages{
          Stage(‘Build’){
          Steps{
            sh ‘make’
          }
          }
       Stage(‘Test’){
        Steps{
          sh ‘make check’
          Junit ‘reports/**/*.xml’
          }
        }
       Stage(‘Deploy’){
          Steps{
            sh ‘make publish’
            }
         }
     }
}
