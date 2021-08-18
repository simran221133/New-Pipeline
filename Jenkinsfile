pipeline {
  agent any
  
    stages {
      stage("Build") {
        steps {
          bash (script: 'docker images -a')
          bash (script: """
            cd azure-vote/
            docker images -a
            docker build -t jenkins-pipeline .
            docker images -a
            cd ..
          """)
        }
      }
      stage("Test") {
        steps {
          echo "Testing an App"
          echo "$GIT_BRANCH"
        }
      }
      stage("Deploy") {
        steps {
          echo "Deploying an App"
          echo "$GIT_BRANCH"
        }
      }
    }
}
