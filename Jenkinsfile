pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
        echo 'Running build automation'
        sh 'chown -cR $USER:$(id -gn $USER) /var/lib/jenkins/tools/com.cloudbees.jenkins.plugins.customtools.CustomTool/micro-gw/wso2am-micro-gw-toolkit-linux-3.2.0/logs/microgw.log.lck'
        sh '/var/lib/jenkins/tools/com.cloudbees.jenkins.plugins.customtools.CustomTool/micro-gw/wso2am-micro-gw-toolkit-linux-3.2.0/bin/micro-gw'
      }
    }
  }
}
