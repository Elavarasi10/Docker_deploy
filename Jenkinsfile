node{
   stage('SCM Checkout'){
     git 'https://github.com/Elavarasi10/Docker_deploy.git'
   }
    stage('Build Docker Image'){
   sh 'docker build -t elavarasi10/myweb:v1.0.'
   }
    stage('Docker Image Push'){
   withCredentials([string(credentialsId: 'dockerhub', variable: 'dockerPassword')]) {
   sh "docker login -u elavarasi10 -p ${dockerPassword}"
    }
   sh 'docker push elavarasi10/myweb:v1.0'
    }
}
