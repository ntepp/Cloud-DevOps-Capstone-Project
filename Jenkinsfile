pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "started"'
             }
         }
		 stage('Lint HTML') {
              steps {
                  sh 'tidy -q -e roles/nginx/templates/*.html'
              }
         } 
     }
}
