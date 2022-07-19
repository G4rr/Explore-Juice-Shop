pipeline {
  agent any 
  stages {
    stage('Scan') {
      steps {
        sh "docker run -v ${WORKSPACE}:/src --workdir /src returntocorp/semgrep semgrep --config=auto /src
      }
    }
  }
}
