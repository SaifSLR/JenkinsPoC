pipeline {
  agent any
  stages {
    node {
  def remote = [:]
  remote.name = 'test'
  remote.host = '192.168.12.137'
  remote.user = 'Admin'
  remote.password = 'Admin123'
  remote.allowAnyHosts = true
  stage('Remote SSH') {
    sshCommand remote: remote, command: "ls -lrt"
    sshCommand remote: remote, command: "for i in {1..5}; do echo -n \"Loop \$i \"; date ; sleep 1; done"
        }
      }
    }
  }
 
 
