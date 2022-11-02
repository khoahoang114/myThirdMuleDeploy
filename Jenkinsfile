pipeline {
  agent {label "linux"}
  stages{
    stage('hello') {
      steps {
        echo 'hello from Jenkinsfile'
      }
    }
    stage('for the branch develop'){
      when{
        branch 'develop'
      }
      steps {
        echo 'deploy UAT'
      }
    }
    stage('for the branch main'){
      when{
        branch 'main'
      }
      steps {
        echo 'deploy PROD'
      }
    }
  }
}
