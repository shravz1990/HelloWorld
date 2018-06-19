pipeline {
     agent any

      stages {

		    stage('build')
        {
      			steps {
        		 sh 'ant all'
     			  }
		    }
	    }

      post {
        always {
          archiveArtifacts artifacts: 'dist/*.war', fingerprint: true
        }
      }
}
