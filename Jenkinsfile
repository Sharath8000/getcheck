pipeline{
    agent {label 'master'}
    //environment {
    // ENV
      //  PATH = "$PATH:/opt/apache-maven-3.8.2/bin"
    //}
    stages{
       stage('GetCode'){
            steps{
                git 'https://github.com/Sharath8000/getcheck.git'
            }
         }        
        stage('Docker image build'){
              steps {
                    sh 'docker build -t firstsapp .'
              }
         }
    }
}
