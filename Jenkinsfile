pipeline {
    agent any
    tools { maven "Maven" }
    stages {
        stage("clone code"){
            steps{
               git branch: 'main', credentialsId: '3f824efe-7afe-4493-be52-c7a930f3ffc5', url: 'https://github.com/shiva42gouda/hello_world.git'
            }
        }
        stage("build code"){
           steps{
              sh "mvn clean install"
            }
       }
      //  stage("deploy"){
        //    steps{
          //    sshagent(['deploy_user']) {
            //     sh "scp -o StrictHostKeyChecking=no webapp/target/webapp.war ec2-user@13.229.183.126:/opt/apache-tomcat-8.5.55/webapps"
                 
              //  }
         //   }
      //  }
    }
}