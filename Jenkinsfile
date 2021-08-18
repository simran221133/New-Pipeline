pipeline {
  agent any
  
    stages {
      stage("Build") {
        steps {
          echo "Building an App"
          echo ${env.GIT_BRANCH}
        }
      }
      stage("Test") {
        steps {
          echo "Testing an App"
          echo ${env.GIT_BRANCH}
        }
      }
      stage("Deploy") {
        steps {
          echo "Deploying an App"
          echo ${env.GIT_BRANCH}
        }
      }
    }
}
