node {
  stage('SCM Checkout'){
    git 'https://github.com/colormaa/my-app'
  } 
  stage('Compile-Package'){
    def mvnHome = tool name: 'maven-3', type: 'maven'
    sh "${mvnHome}/mvn package"
  }
}
