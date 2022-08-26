/* import shared library */
@Library('jenkins-shared-library')_

pipeline {
  agent any
  stages {
    stage ('Start') {
      steps {
        // send build started notifications
      echo "stating the build"
      }
    }
    stage ('Install') {
      steps {
        // install required bundles
        echo "installing require bundles"
      }
    }
    stage ('Build') {
      steps {
        // build
        echo "building the bundles"
      }
    }
    stage ('Test') {
      steps {
        // run tests with coverage
        echo "testing the bundles"
      }
    }
  }
  post {
    always {
      sendNotifications currentBuild.result
    }
  }
}
