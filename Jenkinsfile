pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "started"'
             }
         }
		 stage('Run Test') {
              steps {
                  sh 'tidy -q -e roles/nginx/templates/*.html'
              }
         } 
     }
}
