pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 sh 'echo "Entry step"'
                 sh '''
                     echo "Multiline shell steps works too"
                     ls -lah
                 '''
             }
         }
     }
}
