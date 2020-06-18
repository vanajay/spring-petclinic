pipeline{
agent { docker 'maven:3.6.3-jdk-11' }
    stages{
      stage('Checkout'){ 
      steps{
         git 'https://github.com/vanajay/spring-petclinic.git'
      }
    }
     stage('Build'){
      steps{
          sh 'mvn clean package'
          junit '**/target/surefire-reports/Test-*.xml'
      }

     }
}
       

}
