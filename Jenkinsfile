@Library('my-shared-library@main') _

pipeline {
  agent any
 
 // tools {nodejs "nodejs"}
  parameters {
        string(name: 'url', defaultValue: 'https://github.com/tapasmishraarc/springjavademo.git#main', description: 'My application url')
    }
  stages {
    stage('CI-Pipeline') {
      steps {
        script {
          
        //readProperties "${params.url}", this
      //  echo "${env.APP_NAME}"
         build  "${params.url}", this
        }
        
      }
    }
  }
}

