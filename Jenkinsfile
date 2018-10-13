pipeline {

     agent {
       label 'master'
     }
  

      stages {

		    stage('build'){
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
