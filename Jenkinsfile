pipeline {
  agent any
  stages {
    stage('Fetching Data') {
      steps {
        git(url: 'https://github.com/SaiSindhuManne/Jenkins-Ansible.git', branch: 'main')
      }
    }

    stage('Install Server') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('Deploy App') {
      steps {
        sh 'sudo cp -R * /var/www/html/'
      }
    }

  }
}