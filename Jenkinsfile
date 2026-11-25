pipeline {
  agent any
    stages {
      stage('git clone') {
        steps {
            git branch: 'main', url: 'https://github.com/yogeshbhujbal94699/terraform-jenkins.git'
        }
      }
      stage('terraform init') {
        steps {
            sh 'terraform init'
        }
      }
      stage('terraform plan') {
        steps {
            sh 'terraform plan'
        }
      }
    }
}

