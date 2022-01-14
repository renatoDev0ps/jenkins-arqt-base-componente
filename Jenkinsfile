pipeline {
  agent any
  stages {
    stage('Criando Folder no Jenkins') { 
      steps { 
        script {
          sh "echo 'Criando pasta para o componente'"
          sh "curl -i -k -X POST 'http://192.168.33.10:8080/createItem?name=${NOME_COMPONENTE}&mode=com.cloudbees.hudson.plugins.folder.Folder&from=&json=%7B%22name%22%3A%22FolderName%22%2C%22mode%22%3A%22com.cloudbees.hudson.plugins.folder.Folder%22%2C%22from%22%3A%22%22%2C%22Submit%22%3A%22OK%22%7D&Submit=OK' --user 'devops:11449522f16dfa2b84c1b49713b92df91e' -H 'Jenkins-Crumb:ede7fca7a21253d2112749543f788df6bc08f30c2362079db4c95a676002a0ce' -H 'Content-Type:application/x-www-form-urlencoded'"
        } 
      } 
    }
  }
}
