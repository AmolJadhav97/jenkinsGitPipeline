node {
  def remote = [:]
  remote.name = 'amoljadhav'
  remote.host = '192.168.225.152'
  remote.user = 'amoljadhav'
  remote.password = 'Aj@12697'
  remote.allowAnyHosts = true
  stage('Remote SSH') {
    writeFile file: 'abc.sh', text: 'df -h /dev/sda1'
    sshScript remote: remote, script: "abc.sh"
  }
}
