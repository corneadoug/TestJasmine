node {
    env.NODEJS_HOME = "${tool 'Node 9.2.0'}"
    // on linux / mac
    //env.PATH="${env.NODEJS_HOME}/bin:${env.PATH}"
    // on windows
    env.PATH="${env.NODEJS_HOME};${env.PATH}"
    // test path sh
    env.PATH="${env.PATH};C:\Program Files\Git\bin"
    
    stage('DL') {
      checkout scm
      sh 'npm install'
    }

    stage('Test') {
      sh 'npm test'
    }
}
