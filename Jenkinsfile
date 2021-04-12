node{
stage('scm checkout'){
git branch: 'main', url: 'https://github.com/kumar-devopstraining/maven-project.git' 
}
stage('package'){
def mvnhome = tool name: 'maven', type: 'maven'
sh "${mvnhome}/bin/mvn package"
}
  stage('email notification'){
mail bcc: '', body: '''Hi team
Jenkins job has triggered ''', cc: '', from: '', replyTo: '', subject: 'Jenkins job triggered', to: 'kumar.devopstraining@gmail.com'
}
}
