node {
  stage('SCM Checkout'){
    git 'https://github.com/colormaa/my-app'
  } 
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
  stage('Email notification'){
    mail bcc: '', 
      body: 'hi jenkins', 
      cc: '', from: '', 
      replyTo: '', 
      subject: 'jenkins mail', to: 'bolormaaAmarzayads@gmail.com'
  }
}
