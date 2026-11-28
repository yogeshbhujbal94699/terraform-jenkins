//  ---declarative method-----
pipeline {
  agent any
    stages {
      // stage('git clone') {   <--this stage is optional as already cloned form SCM script
      //   steps {
      //       git branch: 'main', url: 'https://github.com/yogeshbhujbal94699/terraform-jenkins.git'
      //   }
      // }
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
    //   stage('terraform apply') {
    //     steps {
    //         sh 'terraform ${action} -auto-approve'
    //     }
    // }
}
}

// ---scripted method-----
// node {
//       stage('git clone') {   <---this stage is optional as cloned from SCM script
//             git branch: 'main', url: 'https://github.com/yogeshbhujbal94699/terraform-jenkins.git'
//       }
//       stage('terraform init') {
//             sh 'terraform init'
//       }
//       stage('terraform plan') {
//             sh 'terraform plan'
// //      }
//           stage('terraform apply') {
//             sh 'terraform ${action} -auto-approve'
//         }
// }


