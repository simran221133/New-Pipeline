pipeline {
  agent any
  
    stages {
      stage("Build") {
        steps {
          sh "docker run -v /var/run/docker.sock:/var/run/docker.sock ..."
          sh "docker images -a"
          sh (script: """
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
