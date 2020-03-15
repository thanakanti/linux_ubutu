node {
  stage('SCM Checkout') {
        git 'https://github.com/thanakanti/linux_ubutu.git'
        }
   stage('Compile Project'){
     //Get MAVEN HOME PATH
      def mvnHome = tool name: 'MAVEN_HOME', type: 'maven'
      // bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore clean package/)
      //bat "${mvnHome}/bin/mvn -B"
     sh "${mvnHome}/bin/mvn package"
       }
  
  //stage('Quality Check')
 // {
  //withSonarQubeEnv(credentialsId: 'TestingXperts') {
    // some block
//}
  //}
  
 // stage('Sonarqube') {
    
   // environment {
     //   sonarqube = tool 'SonarQubeScanner'
             
       // }
   // }
  
 //stage('SonarQube analysis')
   //{
    //steps
      //{
      //withSonarQubeEnv(credentialsId: 'TestingXperts')
      //{
       // bat 'mvn org.sonarsource.scanner.maven:sonar-maven-plugin:3.6.0.1398:sonar'
      //}
    //}
 // }
   
   // stage('Deploy to Tomcat'){    
//deploy adapters: [tomcat8(credentialsId: 'db3407bc-e68a-4c2f-bc32-b5abd5f67c6d', path: '', url: 'http://localhost:9090')], contextPath: null, war: 'target/Jenkinsfile.war'
//deploy adapters: [tomcat8(credentialsId: 'db3407bc-e68a-4c2f-bc32-b5abd5f67c6d', path: '', url: 'http://localhost:9090')], contextPath: null, war: 'target/*.war'
//  deploy adapters: [tomcat8(credentialsId: 'db3407bc-e68a-4c2f-bc32-b5abd5f67c6d', path: '', url: 'http://localhost:9090')], contextPath: 'rps', war: '**/*.war'
 //deploy adapters: [tomcat8(credentialsId: 'db3407bc-e68a-4c2f-bc32-b5abd5f67c6d', path: '', url: 'http://localhost:9090')], contextPath: 'rps', war: '**/sample.war'
 //   deploy adapters: [tomcat8(credentialsId: 'ae5ff91a-7497-48cf-827d-01500e9a0f95', path: '', url: 'http://localhost:9090')], contextPath: 'rps', war: '**/*.sample.war'
//    deploy adapters: [tomcat8(credentialsId: 'ae5ff91a-7497-48cf-827d-01500e9a0f95', path: '', url: 'http://localhost:9090')], contextPath: 'rps', war: '**/sample.war'
  //    deploy adapters: [tomcat8(credentialsId: 'db3407bc-e68a-4c2f-bc32-b5abd5f67c6d', path: '', url: 'http://localhost:9090')], contextPath: 'rps', war: '**/sample.war'
    //  deploy adapters: [tomcat8(credentialsId: '46bacecd-e89a-4208-9cbe-85cf92615f00', path: '', url: 'http://localhost:9090/')], contextPath: 'rps', war: '**/sample.war'
    //  deploy adapters: [tomcat8(credentialsId: '515c74e4-d208-4728-a348-eeb8bd4c0252', path: '', url: 'http://localhost:9090')], contextPath: 'rps', war: '**/sample.war'
//  }
  stage('Email Notification'){
  mail bcc: '', body: '''Running Pipeline jobs
Thanks
BhanuPrakash''', cc: 'rudrapdas82@gmail.com', from: '', replyTo: '', subject: 'Jenkins Pipeline jobs', to: 'testingwebmail96@gmail.com'
    
   //mail bcc: '', body: '''Hi WELCOME TO JENKINS EMAIL ALERT
   //Thanks Rudra''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'rudrapdas82@gmail.com'
  }  
  stage('Slack Notification') {
   // slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins-pipeline-demo', color: 'good', message: 'welcome to Jenkins slack!', teamDomain: 'RDDEVOPS', tokenCredentialId: 'slack-demo'
  //slackSend botUser: true, channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All, Thanks BhanuPrakash from TestingXperts', notifyCommitters: true, teamDomain: 'devopsteam-ue84413​.slack​.com', username: 'testingwebmail96'
// slackSend baseUrl: 'https://hooks.slack.com/services/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/', channel: 'qa-team', color: 'good ', message: 'Integration of Jenkins with Slack', teamDomain: 'DevopsTeam'
  //  slackSend baseUrl: 'https://hooks.slack.com/services/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/', channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All, Thanks BhanuPrakash from TestingXperts', teamDomain: 'devopsteam-ue84413​.slack​.com', tokenCredentialId: 'hooktoken', username: 'testingwebmail96'
   // slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All, Thanks BhanuPrakash from TestingXperts', teamDomain: 'devopsteam-ue84413​.slack​.com', tokenCredentialId: 'hooktoken', username: 'testingwebmail96'
  //  slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All, Thanks BhanuPrakash from TestingXperts', teamDomain: 'devopsteam-ue84413.slack.com', tokenCredentialId: 'token1', username: 'testingwebmail96'
   // slackSend baseUrl: 'https://hooks.slack.com/services/', botUser: true, channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All, Thanks BhanuPrakash from TestingXperts', teamDomain: 'devopsteam-ue84413.slack.com', tokenCredentialId: 'token1', username: 'testingwebmail96'
   // slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All, Thanks BhanuPrakash from TestingXperts', teamDomain: 'devopsteam-ue84413.slack.com', tokenCredentialId: 'token', username: 'testingwebmail96'
   // slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All , Thanks BhanuPrakash from TestingXperts', teamDomain: 'devopsteam-ue84413.slack.com', tokenCredentialId: 'token', username: 'testingwebmail96'
  //  slackSend baseUrl: 'https://hooks.slack.com/services/', botUser: true, channel: 'qa-team', color: 'good', failOnError: true, message: 'Hi All , Thanks BhanuPrakash from TestingXperts', teamDomain: 'devopsteam-ue84413.slack.com', tokenCredentialId: 'token', username: 'testingwebmail96'
    slackSend baseUrl: 'https://hooks.slack.com/services/', botUser: true, channel: 'qa-team', color: 'good', message: 'Hi All , Thanks BhanuPrakash from TestingXperts', notifyCommitters: true, teamDomain: 'devopsteam-ue84413.slack.com', tokenCredentialId: 'token', username: 'testingwebmail96'
  }
}
