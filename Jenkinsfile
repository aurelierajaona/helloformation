pipeline {
  agent any
  stages {
    stage('stage 1') {
      parallel {
        stage('stage 1') {
          steps {
            sh 'mkdir F1'
          }
        }

        stage('Stage 2') {
          steps {
            sh '''if grep "$user" /etc/passwd > /dev/null
    then
	echo "l\'utilisateur n\'existe pas"
    else
	echo "l\'utilisateur existe"
fi'''
          }
        }

      }
    }

    stage('stage 3') {
      steps {
        sh '''For i in `cat etc/pwd/user`
Do
Ls -il $i
done
'''
      }
    }

  }
}