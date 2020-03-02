pipeline {
   agent any

   stages {
      stage('Build') {
        steps {
          echo 'Building...'
           
           mvn archetype:generate -DarchetypeGroupId=org.apache.maven.archetypes -DarchetypeArtifactId=maven-archetype-webapp -DarchetypeVersion=1.4
           
           echo "Running ${env.BUILD_ID} ${env.BUILD_DISPLAY_NAME} on ${env.NODE_NAME} and JOB ${env.JOB_NAME}"
                   }
   }
   stage('Test') {
     steps {
        echo 'Testing pipeline...'
     }
   }
   stage('Deploy') {
     steps {
       echo 'Deploying. app again..'
     }
   }
  }
}
