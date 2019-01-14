  node{
   stage('SCM Checkout'){
     git 'https://github.com/javahometech/my-app'
   }
   stage('Compile-Package'){
    
      def mvnHome =  tool name: 'maven-3', type: 'maven'   
      sh "${mvnHome}/bin/mvn package"
   }
    stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      Namjith''', cc: '', from: 'namjitharavind@gmail.com', replyTo: '', subject: 'Jenkins Job', to: 'namjitharavind@gmail.com'
   }
  
    
   
}


