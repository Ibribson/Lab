pipeline {
    agent any
    stages {
        stage('Cloner le projet') {
            steps {
                script {
                    if (fileExists('Lab')) {
                        echo 'Mise à jour du dépôt existant...'
                        sh 'cd Lab && git pull origin main'
                    } else {
                        echo 'Clonage du dépôt...'
                        sh 'git clone https://github.com/Ibribson/Lab'
                    }
                }
            }
        }
        stage('Déploiement') {
            steps {
                echo 'Déploiement terminé avec succès !'
            }
        }
    }
}
