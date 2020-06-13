pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
         withAWS(region:'us-east-2', credentials:'aws-static') {
                   s3Upload(bucket:"nalhamid-udacity-project-3", includePathPattern:'**/*');
                }
      }
    }
  }
}
