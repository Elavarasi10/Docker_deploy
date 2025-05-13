node{
   stage('SCM Checkout'){
     git 'https://github.com/Elavarasi10/Jenkins_pipeline.git'
   }
    stage('Build Docker Image'){
   sh 'docker build -t elavarasi10/myweb:v1.0.'
   }
}
