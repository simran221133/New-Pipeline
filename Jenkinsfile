pipeline {
  agent any
  
    stages {
      stage("Build") {
        steps {
<<<<<<< HEAD:jenkinsfile
          sh(script: 'docker images -a')
          sh(script: """
            cd azure-vote/
            docker images -a
            docker build -t jenkins-pipeline .
            docker images -a
            cd ..
          """)
=======
          echo "Building an App"
          echo "$GIT_BRANCH"
>>>>>>> f092ea002cff362884be31ce8ccc13ef34365340:Jenkinsfile
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
