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
          echo "${env.GIT_BRANCH}"
          echo "${env.GIT_LOCAL_BRANCH}"
          echo "${env}"
      }
    }
  }
}
