def getGitBranchName() {
    return scm.branches[0].name
}
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Stage1 - Build"'
      }
    }
    stage('GIT') {
      steps {
        echo getGitBranchName()
      }
    }
  }
}
