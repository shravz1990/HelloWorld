pipeline {

     agent any

      stages {

		    stage('build'){
			steps {
        		 sh 'ant all'
     			  }
		    }
	    }
      post {
       
        always {
           archive 'dist/*.war'
        }
     }
}
