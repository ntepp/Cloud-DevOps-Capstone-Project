pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "started"'
             }
         }
		 stage('Lint Test') {
              steps {
                  sh 'tidy -q -e roles/nginx/templates/*.html'
				  sh hadolint Dockerfile
              }
         }
     }
}
