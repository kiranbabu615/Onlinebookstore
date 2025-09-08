pipeline{
 agent any
 tools{
     maven 'mvn 3.9.0'
 }
 stages{
     stage("CheckOut"){
         steps{
             git branch: 'J2EE', url: 'https://github.com/ChandraSekharAlla/onlinebookstore.git'
         }
     }
     stage("build"){
         steps{
             sh 'mvn clean package'
         }
     }
 }
}
