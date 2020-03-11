pipeline {
   agent any

   stages {
      stage('git-checkout') {
         steps {
            git credentialsId: 'jenkins-git', url: 'https://github.com/devopsankur/JavaHelloWorld.git'
         }
      }
   }
}
