pipeline {
  agent any 
  stages('Scan') {
    steps {
      sh "docker run -v ${WORKSPACE}:/src --workdir /src returntocorp/semgrep-agent semgrep-agent --config p/ci"
    }
  }
}
