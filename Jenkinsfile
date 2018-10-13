pipeline {

     agent none 
  

      stages {

		    stage('build'){
      			agent {
			  label 'master'
			}

			steps {
        		 sh 'ant all'
     			  }
		    }
	    }
     post {
         always {
             archive ‘dist/*.war’
          }
      }

}
