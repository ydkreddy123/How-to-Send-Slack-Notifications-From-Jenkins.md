# How-to-Send-Slack-Notifications-From-Jenkins.md
How-to-Send-Slack-Notifications-From-Jenkins.md

REF: https://plugins.jenkins.io/slack/
REF: https://www.jenkins.io/doc/pipeline/steps/slack/


Sample pipelines



pipeline {
  agent any
  stages {
    stage('Slack') {
      steps {
        slackSend message: 'test message'
      }
    }
  }
}
pipeline {
  agent any
  stages {
    stage('Slack') {
      steps {
        slackSend color: 'good', message: 'test message'
      }
    }
  }
}
