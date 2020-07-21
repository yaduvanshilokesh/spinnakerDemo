node{
stage('Checkout repo'){
git 'https://github.com/yaduvanshilokesh/spinnakerDemo.git'
}
stage('Build and push docker image'){
sh 'docker build -t asia.gcr.io/testproject2-261014/spinnakerdemo:v${BUILD_NUMBER} .'
sh 'docker push asia.gcr.io/testproject2-261014/spinnakerdemo'
}
stage('Create and archive properties file'){
sh label: '', script: 'echo imagetag: v${BUILD_NUMBER} > config.properties'
archive 'config.properties'
}
}
