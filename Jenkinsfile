pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
          echo 'Building...'
           
           javac simplejava.java
          echo "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on ${env.NODE_NAME} and JOB ${env.JOB_NAME}"
           java simplejava.java
        }
   }
   stage('Test') {
     steps {
        echo 'Testing pipeline...'
     }
   }
   stage('Deploy') {
     steps {
       echo 'Deploying...'
     }
   }
  }
}
