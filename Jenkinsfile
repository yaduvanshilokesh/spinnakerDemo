node{
stage('Checkout repo'){
git 'https://github.com/yaduvanshilokesh/spinnakerDemo.git'
}
stage('Build and push docker image'){
sh label: '', script: '''docker build -t asia.gcr.io/testproject2-261014/spinnakerDemo:${env.BUILD_NUMBER} .
docker push asia.gcr.io/testproject2-261014/spinnakerDemo:${env.BUILD_NUMBER}'''
}
}
