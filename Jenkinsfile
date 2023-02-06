pipeline{
  agent any
  stages{
    stage('Setup'){
      steps{
        echo 'Removing previous repo...'
        sh 'sudo rm -rf javaPollingDemo'
        echo 'Cloning repo...'
        sh 'sudo git clone https://github.com/abhimazumder/javaPollingDemo.git'
        sh 'cd javaPollingDemo'
      }
    }
    stage('Compile'){
      steps{
        echo 'Compiling...'
        sh 'sudo javac hello.java'
      }
    }
    stage('Run'){
      steps{
        echo 'Running...'
        sh 'sudo java hello'
      }
    }
  }
}
