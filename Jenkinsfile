pipeline{

  agent { label 'java'
        }
  stages{
    stage('checkout-scm'){
      steps{
        git branch: 'master', credentialsId: 'git-hub-pwd', url: 'https://github.com/divyaraniduggappa/devOpsWeb-Ranjit4github.git'
      }
     }
    stage(maven){
      steps{
         sh 'mvn clean install'  
      
      }
    }
  }
    post{
      success{
        emailext body: 'Here is the test email from smtp server', subject: 'Test Email', to: 'divyarani0911@gmail.com, rakshitha.duggappa@gmail.com'
          }
    }
  }



