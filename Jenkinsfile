pipeline{
       agent any
       stages{
         stage('Éxample Build')
         {
          agent{
          docker 'maven:3.5-alpine'
          }
         steps{
             sh 'mvn --version'
         }
         }
       }

}
