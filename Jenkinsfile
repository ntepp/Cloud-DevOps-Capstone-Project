pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "started"'
             }
         }
		 stage('Lint Html') {
              steps {
                  sh 'tidy -q -e roles/nginx/templates/*.html'
              }
         }
		 stage('Lint Dockerfile') {
              steps {
                  sh 'hadolint Dockerfile'
              }
         }
     }
}
