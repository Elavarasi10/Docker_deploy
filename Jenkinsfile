node{
   stage('SCM Checkout'){
     git 'https://github.com/Elavarasi10/Docker_deploy.git'
   }
    stage('Build Docker Image'){
   sh 'docker build -t elavarasi10/myweb:v1.0.'
   }
}
