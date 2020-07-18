node{
stage('Checkout repo'){
git 'https://github.com/yaduvanshilokesh/spinnakerDemo.git'
}
stage('Build and push docker image'){
sh 'docker build -t asia.gcr.io/testproject2-261014/spinnakerdemo .'
sh 'docker push asia.gcr.io/testproject2-261014/spinnakerdemo'
}
}
