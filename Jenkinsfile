pipeline{

  agent any
  stages{
    stage('Build'){
      steps{
        echo "Building the project pipeline"
      }
     }
    post{
      success{
        emailext body: 'Here is the test email from smtp server', subject: 'Test Email', to: 'divyarani0911@gmail.com, rakshitha.duggappa@gmail.com'
          }
    }
  }
}


