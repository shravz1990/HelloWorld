pipeline {
     agent any
           stages {
                   stage('Build') {
                      steps {
                            sh -c 'ant -f build.xml -v' 
                      }
                   }
            }
}
