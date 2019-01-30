properties([[$class: 'GithubProjectProperty', displayName: '', projectUrlStr: 'https://github.com/vincentsun870530/my-app/'],pipelineTriggers([githubPush()])])  
node{
   stage('SCM Checkout'){
     git 'https://github.com/javahometech/my-app'
   }
  
   stage('Compile-Package'){   
      def mvnHome =  tool name: 'maven-3', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }

   stage('Build'){
     echo "Hello World!!!!"
   }
}


