pipeline {
  agent any
  stages {
    stage('PUSH') {
      steps {
        sh '''echo "from jenkins pipeline" >> a.txt
git add a.txt
git commit a.txt -m "Try cred"
git push origin HEAD:master'''
      }
    }
    stage('FINISH') {
      steps {
        timestamps()
      }
    }
  }
}