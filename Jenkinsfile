sh '''node{
stage (‘scm checkout’) {
git (‘https://github.com/armand0007/docker-cicd.git\')
}
stage (‘Checkout to different branch’) {
sh “git branch -r”
sh “git checkout master”
}
stage (‘package stage’) {
sh label: ‘’, script: ‘mvn clean package ‘
}
}'''