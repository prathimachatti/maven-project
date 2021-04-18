node{
stage('scm checkout'){
git branch: 'main', url: 'https://github.com/prathimachatti/maven-project.git' 
}
stage('package'){
def mvnhome = tool name: 'apache-maven', type: 'maven'
sh "${mvnhome}/bin/mvn package"
}
}

