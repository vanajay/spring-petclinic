pipeline{
       agent { docker 'maven:3.5-alpine'}
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

        stage('checkout')
        {
         steps{

          git  'https://github.com/vanajay/spring-petclinic.git'
        }
       }
       }

}
