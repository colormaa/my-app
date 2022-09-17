node {
  stage('SCM Checkout'){
    tool name: 'maven-3', type: 'maven'
    git 'https://github.com/colormaa/my-app'
  } 
  stage('Compile-Package'){
    sh 'mvn package'
  }
}
